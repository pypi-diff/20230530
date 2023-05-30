# Comparing `tmp/ou_book_theme-0.3.0.tar.gz` & `tmp/ou_book_theme-0.4.0.tar.gz`

## Comparing `ou_book_theme-0.3.0.tar` & `ou_book_theme-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/package-lock.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/rollup.config.js
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/__about__.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/scripts/activity.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/scripts/index.js
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/_activity.scss
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/_time.scss
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/_variables.scss
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/_where-next.scss
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/assets/styles/index.scss
--rw-r--r--   0        0        0    21474 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/cli/__init__.py
--rw-r--r--   0        0        0    40533 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/cli/mermaid-cli/package-lock.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/cli/mermaid-cli/package.json
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/__init__.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/activity.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/time.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/util.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/extensions/where_next.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/theme.conf
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg
--rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/.gitignore
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/README.md
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ou_book_theme-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/package-lock.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/rollup.config.js
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/__about__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/scripts/activity.js
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/scripts/external-link.js
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/scripts/index.js
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_activity.scss
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_external-link.scss
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_time.scss
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_variables.scss
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_where-next.scss
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/index.scss
+-rw-r--r--   0        0        0    22428 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/cli/__init__.py
+-rw-r--r--   0        0        0    40533 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/cli/mermaid-cli/package-lock.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/cli/mermaid-cli/package.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/extensions/__init__.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/extensions/activity.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/extensions/time.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/extensions/where_next.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/theme.conf
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg
+-rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/.gitignore
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/README.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/PKG-INFO
```

### Comparing `ou_book_theme-0.3.0/package-lock.json` & `ou_book_theme-0.4.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.3.0/rollup.config.js` & `ou_book_theme-0.4.0/rollup.config.js`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.3.0/ou_book_theme/__init__.py` & `ou_book_theme-0.4.0/ou_book_theme/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,7 +36,9 @@
     app.add_html_theme('ou_book_theme', theme_dir)
     app.add_js_file('scripts/ou-book-theme.js')
 
     app.connect('html-page-context', hash_js_css_assets)
     app.connect('build-finished', copy_custom_files)
 
     extensions.setup(app)
+
+    return {'parallel_read_safe': True, 'parallel_write_safe': True}
```

### Comparing `ou_book_theme-0.3.0/ou_book_theme/assets/styles/_activity.scss` & `ou_book_theme-0.4.0/ou_book_theme/assets/styles/_activity.scss`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.3.0/ou_book_theme/assets/styles/_where-next.scss` & `ou_book_theme-0.4.0/ou_book_theme/assets/styles/_where-next.scss`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         &::before {
             position: absolute;
             left: .6rem;
             width: 1rem;
             height: 1rem;
             color: rgba(var(--ou-color-where-next),1);
-            font-family: 'Font Awesome 5 Free';
+            font-family: 'Font Awesome 6 Free';
             font-weight: 400;
             content: var(--ou-icon-where-next);
         }
 
         + * {
             margin-top: .4rem;
         }
```

### Comparing `ou_book_theme-0.3.0/ou_book_theme/cli/__init__.py` & `ou_book_theme-0.4.0/ou_book_theme/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,63 @@
+"""OU Book Theme CLI application."""
 import typer
 
 from datetime import datetime
 from importlib.resources import files, as_file
 from lxml import etree
 from os import path, makedirs
 from rich import print as stdout
 from rich.progress import Progress
 from shutil import rmtree, copy
 from subprocess import run
 from yaml import safe_load
 
+from ..__about__ import __version__
+
+
+app = typer.Typer()
+
 
 def xpath_single(start: etree.Element, xpath: str):
+    """Retrieve a single element using XPath."""
     return start.xpath(xpath)[0]
 
 
 def create_text_node(tag: str, text: str) -> etree.Element:
+    """Create a new text node."""
     element = etree.Element(tag)
     element.text = text
     return element
 
 
 def fix_sub_list(node: etree.Element):
+    """Fix the nested list tags."""
     # Fix sub lists so that they use the correct tags
     if node.tag == 'BulletedList':
         node.tag = 'BulletedSubsidiaryList'
     elif node.tag == 'NumberedList':
         node.tag = 'NumberedSubsidiaryList'
     elif node.tag == 'ListItem':
         node.tag = 'SubListItem'
     for child in node:
         fix_sub_list(child)
 
 
-def apply_fixes(config: dict, source: str, node: etree.Element, module_code: str, block: int, part: int, presentation: str, counters: dict, part_title: str) -> None:
+def apply_fixes(
+        config: dict,
+        source: str,
+        node: etree.Element,
+        module_code: str,
+        block: int,
+        part: int,
+        presentation: str,
+        counters: dict,
+        part_title: str
+    ) -> None:
+    """Apply a range of post-processing fixes."""
     # Postprocessing required:
     # * Remove non-document cross-links
     if node.tag == 'ComputerDisplayBlock':
         # Add paragraphs into block-level computer displays
         node.tag = 'ComputerDisplay'
         lines = node.text.split('\n')
         if lines[-1].strip() == '':
@@ -149,14 +169,15 @@
         apply_fixes(config, source, child, module_code, block, part, presentation, counters, part_title)
 
 
 def transform_content(
         node: etree.Element,
         root_node: str='Section'
     ) -> etree.Element:
+    """Apply the XSLT transforms from Sphinx XML to OU XML."""
     stylesheet = etree.XML(f'''\
 <xsl:stylesheet version="1.0" xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
     <!-- Section templates -->
     <xsl:template match="/section">
         <{root_node}><xsl:apply-templates/></{root_node}>
     </xsl:template>
     <xsl:template match="section">
@@ -331,59 +352,64 @@
     </xsl:template>
 </xsl:stylesheet>''')
     transform = etree.XSLT(stylesheet)
     return transform(xpath_single(node, '/document/section')).getroot()
 
 
 def create_introduction(input_base: str, root: etree.Element, block: int, part: dict, chapter: dict) -> None:
+    """Create the introduction structure."""
     with open(path.join(input_base, f'{chapter["file"]}.xml')) as in_f:
         doc = etree.parse(in_f)
         root.append(transform_content(
             doc,
             root_node='Introduction'
         ))
 
 
 def create_section(input_base: str, root: etree.Element, section: dict) -> None:
+    """Create the structure for a single section, which writes to a single part file."""
     with open(path.join(input_base, f'{section["file"]}.xml')) as in_f:
         doc = etree.parse(in_f)
         section = transform_content(
             doc,
             root_node='Section'
         )
         root.append(section)
 
 
 def create_session(input_base: str, root: etree.Element, chapter: dict) -> None:
+    """Create a sesssion within a file."""
     with open(path.join(input_base, f'{chapter["file"]}.xml')) as in_f:
         doc = etree.parse(in_f)
         session = transform_content(
             doc,
             root_node='Session'
         )
         if 'sections' in chapter:
             for section in chapter['sections']:
                 create_section(input_base, session, section)
         root.append(session)
 
 
 def create_unit(config: dict, root: etree.Element, part: dict, input_base: str, block: int) -> None:
+    """Create a single unit."""
     unit = etree.Element('Unit')
     root.append(unit)
     unit.append(create_text_node('UnitID', f'Block {block}: {config["ou"]["block_title"]}'))
     unit.append(create_text_node('UnitTitle', f'{part["caption"]}: $PART_TITLE'))
     unit.append(create_text_node('ByLine', config['author']))
     for chapter_idx, chapter in enumerate(part['chapters']):
         if chapter_idx == 0:
             create_introduction(input_base, unit, block, part, chapter)
         else:
             create_session(input_base, unit, chapter)
 
 
 def create_frontmatter(root: etree.Element, config: dict) -> None:
+    """Create the frontmatter XML structure."""
     frontmatter = etree.XML(f'''\
 <FrontMatter>
   <ByLine>{config["author"]}</ByLine>
   <Imprint>
     <Standard>
       <GeneralInfo>
         <Paragraph>This publication forms part of the Open University module {config["ou"]["module_code"]} {config["ou"]["module_title"]}. [The complete list of texts which make up this module can be found at the back (where applicable)]. Details of this and other Open University modules can be obtained from the Student Registration and Enquiry Service, The Open University, PO Box 197, Milton Keynes MK7 6BJ, United Kingdom (tel. +44 (0)845 300 60 90; email general-enquiries@open.ac.uk).</Paragraph>
@@ -423,14 +449,15 @@
   </Imprint>
 </FrontMatter>
 ''')
     root.append(frontmatter)
 
 
 def create_root(config: dict, part_idx: int) -> etree.Element:
+    """Create the root structure."""
     module_code = config['ou']['module_code']
     module_title = config['ou']['module_title']
     block = int(config['ou']['block'])
     presentation = config['ou']['presentation']
 
     root = etree.Element('Item')
     root.attrib['TextType'] = 'CompleteItem'
@@ -448,15 +475,17 @@
     root.append(create_text_node('CourseTitle', module_title))
     root.append(etree.Element('ItemID'))
     root.append(create_text_node('ItemTitle', f'Block {block}, Part {part_idx}: $PART_TITLE'))
 
     return root
 
 
-def convert(source: str, regenerate: bool=False):
+@app.command()
+def convert_to_ouxml(source: str, regenerate: bool=False, numbering_from: int=1):
+    """Convert the content into OU XML."""
     input_base = path.join(source, '_build', 'xml')
     if not path.exists(input_base) or regenerate:
         result = run(['jb', 'build', '--builder', 'custom', '--custom-builder', 'xml', source])
         stdout('')
         if result.returncode == 0:
             stdout('[green]XML (re)built[/green] ✓')
             stdout('')
@@ -482,19 +511,27 @@
         progress.update(clearing_task, completed=3)
 
         main_task = progress.add_task('Converting', total=len(toc['parts']))
         module_code = config['ou']['module_code']
         block = int(config['ou']['block'])
         presentation = config['ou']['presentation']
         for part_idx, part in enumerate(toc['parts']):
+            part_idx = numbering_from + part_idx
             root = create_root(config, part_idx)
             create_frontmatter(root, config)
             create_unit(config, root, part, input_base, block)
             part_title = xpath_single(root, '/Item/Unit/Introduction/Title/text()')
             apply_fixes(config, source, root, module_code, block, part_idx, presentation, {'session': 0, 'section': 0, 'figure': 0, 'table': 0}, part_title)
             with open(path.join(output_base, f'{module_code.lower()}_b{block}_p{part_idx}_{presentation.lower()}.xml'), 'wb') as out_f:
                 out_f.write(etree.tostring(root, pretty_print=True, encoding='utf-8', xml_declaration=True))
             progress.update(main_task, advance=1)
 
 
+@app.command()
+def version():
+    """Print the current version."""
+    stdout(__version__)
+
+
 def main():
-    typer.run(convert)
+    """Run the OBT application."""
+    app()
```

### Comparing `ou_book_theme-0.3.0/ou_book_theme/cli/mermaid-cli/package-lock.json` & `ou_book_theme-0.4.0/ou_book_theme/cli/mermaid-cli/package-lock.json`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.3.0/ou_book_theme/extensions/activity.py` & `ou_book_theme-0.4.0/ou_book_theme/extensions/activity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Additional Sphinx directives for OU activities."""
 from docutils import nodes
 from sphinx.util.docutils import SphinxDirective
 from sphinx.transforms.post_transforms import SphinxPostTransform
 from sphinx_design.shared import is_component, create_component
 
 
 class ActivityDirective(SphinxDirective):
@@ -99,8 +100,7 @@
 
 def setup(app):
     """Setup the Activity extensions."""
     app.add_directive('activity', ActivityDirective)
     app.add_directive('activity-answer', ActivityAnswerDirective)
     app.add_post_transform(ActivityHtmlTransform)
     app.add_post_transform(ActivityAnswerHtmlTransform)
-    return {'parallel_read_safe': True, 'parallel_write_safe': True}
```

### Comparing `ou_book_theme-0.3.0/ou_book_theme/extensions/where_next.py` & `ou_book_theme-0.4.0/ou_book_theme/extensions/where_next.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Additional Sphinx directives for the where-next blocks."""
 from docutils import nodes
 from sphinx.util.docutils import SphinxDirective
 from sphinx.transforms.post_transforms import SphinxPostTransform
 from sphinx_design.shared import is_component, create_component
 
 
 class WhereNextDirective(SphinxDirective):
@@ -64,8 +65,7 @@
         self.set_class('ou-where-next-content')
 
 
 def setup(app):
     """Setup the Where Next extensions."""
     app.add_directive('where-next', WhereNextDirective)
     app.add_post_transform(WhereNextHtmlTransform)
-    return {'parallel_read_safe': True, 'parallel_write_safe': True}
```

### Comparing `ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg` & `ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg` & `ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.3.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css` & `ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 @charset "UTF-8";
 @import "sphinx-book-theme.css";
 :root {
   --ou-color-activity: 98, 191, 178;
   --ou-color-where-next: 45, 187, 235;
   --ou-icon-time: "";
   --ou-icon-where-next: "";
+  --ou-icon-external-link: "";
 }
 
 html[data-theme=light] {
   --pst-color-inline-code: #cd1468;
 }
 
 html[data-theme=light] {
@@ -87,15 +88,15 @@
 }
 .ou-time::before {
   position: absolute;
   left: 0.3rem;
   width: 1rem;
   height: 1rem;
   color: currentColor;
-  font-family: "Font Awesome 5 Free";
+  font-family: "Font Awesome 6 Free";
   font-weight: 400;
   font-style: normal;
   content: var(--ou-icon-time);
 }
 
 .ou-where-next {
   margin: 1.5625em auto;
@@ -120,25 +121,34 @@
 }
 .ou-where-next .ou-where-next-title::before {
   position: absolute;
   left: 0.6rem;
   width: 1rem;
   height: 1rem;
   color: rgba(var(--ou-color-where-next), 1);
-  font-family: "Font Awesome 5 Free";
+  font-family: "Font Awesome 6 Free";
   font-weight: 400;
   content: var(--ou-icon-where-next);
 }
 .ou-where-next .ou-where-next-title + * {
   margin-top: 0.4rem;
 }
 .ou-where-next .ou-where-next-title ~ * {
   margin-left: 1.4rem;
   margin-right: 1.4rem;
 }
 .ou-where-next > :last-child {
   margin-bottom: 0;
 }
 
+a.reference.external::after {
+  padding-left: 0.3rem;
+  color: currentColor;
+  font-family: "Font Awesome 6 Free";
+  font-style: normal;
+  font-weight: 900;
+  content: var(--ou-icon-external-link);
+}
+
 article a {
   text-decoration: underline dotted;
 }
```

### Comparing `ou_book_theme-0.3.0/pyproject.toml` & `ou_book_theme-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.3.0/PKG-INFO` & `ou_book_theme-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ou-book-theme
-Version: 0.3.0
+Version: 0.4.0
 Project-URL: Documentation, https://github.com/unknown/ou-book-theme#readme
 Project-URL: Issues, https://github.com/unknown/ou-book-theme/issues
 Project-URL: Source, https://github.com/unknown/ou-book-theme
 Author-email: Mark Hall <mark.hall@open.ac.uk>
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

