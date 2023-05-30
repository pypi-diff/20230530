# Comparing `tmp/genopyc-0.2.333-py3-none-any.whl.zip` & `tmp/genopyc-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17849 bytes, number of entries: 7
+Zip file size: 18320 bytes, number of entries: 7
 -rwxrwxrwx  2.0 unx      797 b- defN 23-Mar-21 18:10 genopyc/__init__.py
--rwxrwxrwx  2.0 unx    21797 b- defN 23-Mar-27 13:03 genopyc/genopyc.py
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Mar-27 13:09 genopyc-0.2.333.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      465 b- defN 23-Mar-27 13:09 genopyc-0.2.333.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Mar-27 13:09 genopyc-0.2.333.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Mar-27 13:09 genopyc-0.2.333.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      550 b- defN 23-Mar-27 13:09 genopyc-0.2.333.dist-info/RECORD
-7 files, 58232 bytes uncompressed, 16875 bytes compressed:  71.0%
+-rwxrwxrwx  2.0 unx    23926 b- defN 23-May-30 13:09 genopyc/genopyc.py
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-May-30 13:12 genopyc-0.2.4.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      463 b- defN 23-May-30 13:12 genopyc-0.2.4.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-May-30 13:12 genopyc-0.2.4.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-May-30 13:12 genopyc-0.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      540 b- defN 23-May-30 13:12 genopyc-0.2.4.dist-info/RECORD
+7 files, 60349 bytes uncompressed, 17366 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: genopyc/__init__.py
 Comment: 
 
 Filename: genopyc/genopyc.py
 Comment: 
 
-Filename: genopyc-0.2.333.dist-info/LICENSE.txt
+Filename: genopyc-0.2.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-0.2.333.dist-info/METADATA
+Filename: genopyc-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-0.2.333.dist-info/WHEEL
+Filename: genopyc-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-0.2.333.dist-info/top_level.txt
+Filename: genopyc-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-0.2.333.dist-info/RECORD
+Filename: genopyc-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/genopyc.py

```diff
@@ -566,9 +566,71 @@
                     pass
         try:
             return min([(k,np.absolute(v)) for (k,v) in elements.items()], key=lambda x:x[1])
         except:
             return 'no_genes'
 
 
+        
+def ConvertVariants(ListOfVariants,source='variantid',target='rsid'):
+    
+    OT_url='https://api.genetics.opentargets.org/graphql'
+    MappingDict={}
+    if (source=='variantid') & (target=='rsid'):
+        query="""{
+               variantInfo(variantId:"%s"){
+                   rsId
+                   }
+              }"""
+        for variant in ListOfVariants:
+            r = requests.post(OT_url, json={'query': query % (variant)})
+            JsonResponse=r.json()
+            MappingDict[variant]=JsonResponse['data']['variantInfo']['rsId']
+        return list(map(MappingDict.get,ListOfVariants))
+
+    elif (source=='rsid') & (target=='variantid'):
+        query="""{
+              search(queryString:"%s"){
+                  variants{
+                      id
+                      }
+                   }
+              }
+              """
+        for variant in ListOfVariants:
+            r = requests.post(OT_url, json={'query': query % (variant)})
+            JsonResponse=r.json()
+            MappingDict[variant]=JsonResponse['data']['search']['variants'][0]['id']
+        return list(map(MappingDict.get,ListOfVariants))
+
+
+    
+def OTVariantsToGenes(ListofVariants,score=0.1,output='genes'):
+    query="""{
+              genesForVariant(variantId:"%s"){
+                overallScore
+                gene{id}
+              }
+            }
+            """
+    OT_url='https://api.genetics.opentargets.org/graphql'
+    
+    results={}
+    for variant in ListofVariants:
+        r = requests.post(OT_url, json={'query': query % (variant)})
+        r = r.json()
+        ResultsForVariant=[]
+        for data in r['data']['genesForVariant']:
+            ResultsForVariant.append((data['gene']['id'],data['overallScore']))
+        results[variant]=ResultsForVariant
+    if output=='all':
+        return results
+    elif output=='GenScor':
+        return {key:[value for value in values if value[1]>score] for (key,values) in results.items()}
+    else:
+        return list(set(sum([[value[0] for value in values if value[1]>score] for (key,values) in results.items()],[])))
+    
+            
+            
+
```

## Comparing `genopyc-0.2.333.dist-info/LICENSE.txt` & `genopyc-0.2.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

