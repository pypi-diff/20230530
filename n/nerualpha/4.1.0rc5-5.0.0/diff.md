# Comparing `tmp/nerualpha-4.1.0rc5.tar.gz` & `tmp/nerualpha-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerualpha-4.1.0rc5.tar", max compression
+gzip compressed data, was "nerualpha-5.0.0.tar", max compression
```

## Comparing `nerualpha-4.1.0rc5.tar` & `nerualpha-5.0.0.tar`

### file list

```diff
@@ -1,446 +1,446 @@
--rw-r--r--   0        0        0      594 2023-04-11 15:54:47.931455 nerualpha-4.1.0rc5/README.md
--rw-r--r--   0        0        0      843 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/pyproject.toml
--rw-r--r--   0        0        0     1708 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/IBridge.py
--rw-r--r--   0        0        0      853 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/INeru.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/__init__.py
--rw-r--r--   0        0        0     4323 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/bridge.py
--rw-r--r--   0        0        0     3926 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/neru.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/IAssets.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/__init__.py
--rw-r--r--   0        0        0     5963 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/assets.py
--rw-r--r--   0        0        0      316 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/assetsActions.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetInfo.py
--rw-r--r--   0        0        0     1083 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetLinkResponse.py
--rw-r--r--   0        0        0     1149 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetListResponse.py
--rw-r--r--   0        0        0     1100 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/directoryPayload.py
--rw-r--r--   0        0        0     1087 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/getAssetPayload.py
--rw-r--r--   0        0        0     1098 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/getAssetResponse.py
--rw-r--r--   0        0        0     1145 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/linkPayload.py
--rw-r--r--   0        0        0     1212 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/listAssetsPayload.py
--rw-r--r--   0        0        0     1165 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/removeAssetPayload.py
--rw-r--r--   0        0        0      334 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/assets/fileRetentionPeriod.py
--rw-r--r--   0        0        0      304 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/IEventEmitter.py
--rw-r--r--   0        0        0      312 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/IEventFactory.py
--rw-r--r--   0        0        0      388 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/INeruEvent.py
--rw-r--r--   0        0        0      200 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/ISessionCreatedDetails.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/__init__.py
--rw-r--r--   0        0        0     2804 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/eventEmitter.py
--rw-r--r--   0        0        0     2389 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/eventFactory.py
--rw-r--r--   0        0        0     1348 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/neruEvent.py
--rw-r--r--   0        0        0      189 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/neruEventSourceTypes.py
--rw-r--r--   0        0        0      477 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/neruEventTypes.py
--rw-r--r--   0        0        0     1224 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/events/sessionCreatedDetails.py
--rw-r--r--   0        0        0      447 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/ILogAction.py
--rw-r--r--   0        0        0      221 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/ILogContext.py
--rw-r--r--   0        0        0      311 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/ILogger.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/__init__.py
--rw-r--r--   0        0        0     1415 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logAction.py
--rw-r--r--   0        0        0     1292 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logContext.py
--rw-r--r--   0        0        0      228 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logLevels.py
--rw-r--r--   0        0        0     2990 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logger.py
--rw-r--r--   0        0        0      212 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/logger/sourceTypes.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/__init__.py
--rw-r--r--   0        0        0      199 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/ICreateRoomPayload.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/__init__.py
--rw-r--r--   0        0        0     1667 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/createRoomPayload.py
--rw-r--r--   0        0        0     1055 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/deleteRoomPayload.py
--rw-r--r--   0        0        0     1274 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/getRoomsResponse.py
--rw-r--r--   0        0        0     1194 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/pageLinks.py
--rw-r--r--   0        0        0     1111 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/recordingOptions.py
--rw-r--r--   0        0        0     1158 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomLinks.py
--rw-r--r--   0        0        0     1465 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomResponse.py
--rw-r--r--   0        0        0     1158 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomsEmbedded.py
--rw-r--r--   0        0        0     1208 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/updateRoomDetails.py
--rw-r--r--   0        0        0     1232 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/updateRoomPayload.py
--rw-r--r--   0        0        0     3288 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/meetings.py
--rw-r--r--   0        0        0      203 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/roomTypes.py
--rw-r--r--   0        0        0     1596 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/IMessages.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/__init__.py
--rw-r--r--   0        0        0      234 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IBaseMessage.py
--rw-r--r--   0        0        0      198 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IImageData.py
--rw-r--r--   0        0        0      495 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IListenEventsPayload.py
--rw-r--r--   0        0        0      497 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IListenMessagesPayload.py
--rw-r--r--   0        0        0      359 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMMSAudioMessage.py
--rw-r--r--   0        0        0      359 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMMSImageMessage.py
--rw-r--r--   0        0        0      359 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMMSVCardMessage.py
--rw-r--r--   0        0        0      359 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMMSVideoMessage.py
--rw-r--r--   0        0        0      215 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessageContact.py
--rw-r--r--   0        0        0      199 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessenger.py
--rw-r--r--   0        0        0      365 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerAudioMessage.py
--rw-r--r--   0        0        0      363 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerFileMessage.py
--rw-r--r--   0        0        0      365 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerImageMessage.py
--rw-r--r--   0        0        0      194 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerTextMessage.py
--rw-r--r--   0        0        0      365 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IMessengerVideoMessage.py
--rw-r--r--   0        0        0      270 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISMSMessage.py
--rw-r--r--   0        0        0      285 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendImageContent.py
--rw-r--r--   0        0        0      294 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendImageMessage.py
--rw-r--r--   0        0        0      426 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendImagePayload.py
--rw-r--r--   0        0        0      276 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendImageResponse.py
--rw-r--r--   0        0        0      194 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendResponse.py
--rw-r--r--   0        0        0      203 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendTextContent.py
--rw-r--r--   0        0        0      297 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendTextMessagePayload.py
--rw-r--r--   0        0        0      443 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/ISendTextPayload.py
--rw-r--r--   0        0        0      199 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IURLPayload.py
--rw-r--r--   0        0        0      196 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IUnsubscribeEventsPayload.py
--rw-r--r--   0        0        0      361 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IViberImageMessage.py
--rw-r--r--   0        0        0      216 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IViberService.py
--rw-r--r--   0        0        0      276 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IViberTextMessage.py
--rw-r--r--   0        0        0      199 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsapp.py
--rw-r--r--   0        0        0      364 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappAudioMessage.py
--rw-r--r--   0        0        0      362 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappFileMessage.py
--rw-r--r--   0        0        0      364 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappImageMessage.py
--rw-r--r--   0        0        0      215 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappTemplate.py
--rw-r--r--   0        0        0      482 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappTemplateMessage.py
--rw-r--r--   0        0        0      279 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappTextMessage.py
--rw-r--r--   0        0        0      364 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/IWhatsappVideoMessage.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/__init__.py
--rw-r--r--   0        0        0     1206 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/baseMessage.py
--rw-r--r--   0        0        0     1220 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/imageData.py
--rw-r--r--   0        0        0     1492 2023-04-11 15:54:47.935454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/listenEventsPayload.py
--rw-r--r--   0        0        0     1500 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/listenMessagesPayload.py
--rw-r--r--   0        0        0     1202 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messageContact.py
--rw-r--r--   0        0        0     1508 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerAudioMessage.py
--rw-r--r--   0        0        0     1502 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerFileMessage.py
--rw-r--r--   0        0        0     1508 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerImageMessage.py
--rw-r--r--   0        0        0     1419 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerTextMessage.py
--rw-r--r--   0        0        0     1508 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerVideoMessage.py
--rw-r--r--   0        0        0     1385 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsAudioMessage.py
--rw-r--r--   0        0        0     1372 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsImageMessage.py
--rw-r--r--   0        0        0     1372 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsVCardMessage.py
--rw-r--r--   0        0        0     1372 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsVideoMessage.py
--rw-r--r--   0        0        0     1330 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImageContent.py
--rw-r--r--   0        0        0     1309 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImageMessage.py
--rw-r--r--   0        0        0     1679 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImagePayload.py
--rw-r--r--   0        0        0     1166 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendResponse.py
--rw-r--r--   0        0        0     1235 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextContent.py
--rw-r--r--   0        0        0     1330 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextMessagePayload.py
--rw-r--r--   0        0        0     1729 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextPayload.py
--rw-r--r--   0        0        0     1267 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/smsMessage.py
--rw-r--r--   0        0        0     1220 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/unsubscribeEventsPayload.py
--rw-r--r--   0        0        0     1173 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/urlPayload.py
--rw-r--r--   0        0        0     1509 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/viberImageMessage.py
--rw-r--r--   0        0        0     1420 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/viberTextMessage.py
--rw-r--r--   0        0        0     1397 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappAudioMessage.py
--rw-r--r--   0        0        0     1391 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappFileMessage.py
--rw-r--r--   0        0        0     1397 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappImageMessage.py
--rw-r--r--   0        0        0     1528 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappTemplateMessage.py
--rw-r--r--   0        0        0     1308 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappTextMessage.py
--rw-r--r--   0        0        0     1397 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappVideoMessage.py
--rw-r--r--   0        0        0      317 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messageActions.py
--rw-r--r--   0        0        0      219 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messageChannelType.py
--rw-r--r--   0        0        0      298 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messageType.py
--rw-r--r--   0        0        0     4786 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messages.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/__init__.py
--rw-r--r--   0        0        0      187 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/IBaseNumberOptions.py
--rw-r--r--   0        0        0      411 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/IGetNumbersOptions.py
--rw-r--r--   0        0        0      331 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/INumberOptions.py
--rw-r--r--   0        0        0      403 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/ISearchNumbersOptions.py
--rw-r--r--   0        0        0      450 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/IUpdateNumberOptions.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/__init__.py
--rw-r--r--   0        0        0     1163 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/baseNumberOptions.py
--rw-r--r--   0        0        0     1453 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/getNumbersOptions.py
--rw-r--r--   0        0        0     1185 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/getNumbersResponse.py
--rw-r--r--   0        0        0     1315 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numberOptions.py
--rw-r--r--   0        0        0     1259 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numberResponse.py
--rw-r--r--   0        0        0     1129 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numbersOperationResponse.py
--rw-r--r--   0        0        0     1515 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/searchNumbersOptions.py
--rw-r--r--   0        0        0     1492 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/updateNumberOptions.py
--rw-r--r--   0        0        0      208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/numberFeature.py
--rw-r--r--   0        0        0     7697 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/numbers.py
--rw-r--r--   0        0        0     1672 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/IQueue.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/__init__.py
--rw-r--r--   0        0        0      236 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/ICreateQueueOptions.py
--rw-r--r--   0        0        0      392 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/ICreateQueuePayload.py
--rw-r--r--   0        0        0      386 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IQueueDetails.py
--rw-r--r--   0        0        0      280 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IQueueDetailsStats.py
--rw-r--r--   0        0        0      211 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IQueueRate.py
--rw-r--r--   0        0        0      220 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IUpdateQueueOptions.py
--rw-r--r--   0        0        0      269 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/IUpdateQueuePayload.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/createQueueOptions.py
--rw-r--r--   0        0        0     1382 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/createQueuePayload.py
--rw-r--r--   0        0        0      402 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/queueDetailsResponse.py
--rw-r--r--   0        0        0     1172 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/queueRate.py
--rw-r--r--   0        0        0     1208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/updateQueueOptions.py
--rw-r--r--   0        0        0     1256 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/updateQueuePayload.py
--rw-r--r--   0        0        0     6959 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/queue/queue.py
--rw-r--r--   0        0        0     1044 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/IScheduler.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/__init__.py
--rw-r--r--   0        0        0      289 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IIntervalParams.py
--rw-r--r--   0        0        0      208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IListAllPayload.py
--rw-r--r--   0        0        0      187 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/ISchedulePayload.py
--rw-r--r--   0        0        0      374 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IStartAtParams.py
--rw-r--r--   0        0        0      447 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IStartAtPayload.py
--rw-r--r--   0        0        0      208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/IUntilParams.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/__init__.py
--rw-r--r--   0        0        0     1381 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/getSchedulerResponse.py
--rw-r--r--   0        0        0     1269 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/intervalParams.py
--rw-r--r--   0        0        0     1305 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/listAllPayload.py
--rw-r--r--   0        0        0     1123 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/listAllSchedulersResponse.py
--rw-r--r--   0        0        0     1138 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/schedulerExecutionInfo.py
--rw-r--r--   0        0        0     1186 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/schedulerPayload.py
--rw-r--r--   0        0        0     1375 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/startAtParams.py
--rw-r--r--   0        0        0     1456 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/startAtPayload.py
--rw-r--r--   0        0        0     1179 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/untilParams.py
--rw-r--r--   0        0        0     3999 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/scheduler.py
--rw-r--r--   0        0        0      237 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/schedulerActions.py
--rw-r--r--   0        0        0     1971 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/IState.py
--rw-r--r--   0        0        0      240 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/IStateCommand.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/__init__.py
--rw-r--r--   0        0        0      212 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/expireOptions.py
--rw-r--r--   0        0        0     9864 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/state.py
--rw-r--r--   0        0        0     1341 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/stateCommand.py
--rw-r--r--   0        0        0      694 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/state/stateOperations.py
--rw-r--r--   0        0        0     4370 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IConversation.py
--rw-r--r--   0        0        0     1208 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IUsers.py
--rw-r--r--   0        0        0     1636 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IVoice.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/__init__.py
--rw-r--r--   0        0        0      207 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/callDirections.py
--rw-r--r--   0        0        0      257 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/callStatuses.py
--rw-r--r--   0        0        0      344 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAcceptInboundCallBody.py
--rw-r--r--   0        0        0      215 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAcceptInboundCallEndpoint.py
--rw-r--r--   0        0        0      403 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAcceptInboundCallEvent.py
--rw-r--r--   0        0        0      460 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAcceptInboundCallPayload.py
--rw-r--r--   0        0        0      209 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAddUserPayload.py
--rw-r--r--   0        0        0      225 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IAudioSettings.py
--rw-r--r--   0        0        0      536 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannel.py
--rw-r--r--   0        0        0      190 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannelEndpoint.py
--rw-r--r--   0        0        0      291 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannelPhoneEndpoint.py
--rw-r--r--   0        0        0      346 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannelSIPEndpoint.py
--rw-r--r--   0        0        0      292 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannelVBCEndpoint.py
--rw-r--r--   0        0        0      304 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IConversationPayloadWithCallback.py
--rw-r--r--   0        0        0      220 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ICreateConversationPayload.py
--rw-r--r--   0        0        0      250 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ICreateUserPayload.py
--rw-r--r--   0        0        0      277 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IDeleteMemberPayload.py
--rw-r--r--   0        0        0      214 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IEarmuffPayload.py
--rw-r--r--   0        0        0      371 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IInviteMemberPayload.py
--rw-r--r--   0        0        0      179 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ILeg.py
--rw-r--r--   0        0        0      293 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IMedia.py
--rw-r--r--   0        0        0      211 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IMutePayload.py
--rw-r--r--   0        0        0      423 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IOnInboundCallPayload.py
--rw-r--r--   0        0        0      189 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IPlayStopBody.py
--rw-r--r--   0        0        0      300 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IPlayStopPayload.py
--rw-r--r--   0        0        0      241 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IPlayStreamBody.py
--rw-r--r--   0        0        0      308 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IPlayStreamPayload.py
--rw-r--r--   0        0        0      193 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IReason.py
--rw-r--r--   0        0        0      187 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayStopBody.py
--rw-r--r--   0        0        0      296 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayStopPayload.py
--rw-r--r--   0        0        0      291 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayTextBody.py
--rw-r--r--   0        0        0      293 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayTextParams.py
--rw-r--r--   0        0        0      285 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ISayTextPayload.py
--rw-r--r--   0        0        0      373 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/ITransferMemberPayload.py
--rw-r--r--   0        0        0      250 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IUpdateUserPayload.py
--rw-r--r--   0        0        0      251 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IUser.py
--rw-r--r--   0        0        0      277 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiAnswerCallBack.py
--rw-r--r--   0        0        0      274 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiCreateCallOptions.py
--rw-r--r--   0        0        0      373 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiCreateCallPayload.py
--rw-r--r--   0        0        0      312 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiEventCallBackPayload.py
--rw-r--r--   0        0        0      233 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IVapiEventParams.py
--rw-r--r--   0        0        0     1063 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/Link.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallBody.py
--rw-r--r--   0        0        0     1224 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallEndpoint.py
--rw-r--r--   0        0        0     1407 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallEvent.py
--rw-r--r--   0        0        0     1824 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallPayload.py
--rw-r--r--   0        0        0     1240 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/addUserPayload.py
--rw-r--r--   0        0        0     1351 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/addUserResponse.py
--rw-r--r--   0        0        0     1261 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSayResponseBody.py
--rw-r--r--   0        0        0     1078 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSayStopResponseBody.py
--rw-r--r--   0        0        0     1308 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSettings.py
--rw-r--r--   0        0        0     1605 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channel.py
--rw-r--r--   0        0        0     1315 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelAppEndpoint.py
--rw-r--r--   0        0        0     1342 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelPhoneEndpoint.py
--rw-r--r--   0        0        0     1626 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelSIPEndpoint.py
--rw-r--r--   0        0        0     1344 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelVBCEndpoint.py
--rw-r--r--   0        0        0     1430 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/conversationPayloadWithCallback.py
--rw-r--r--   0        0        0     1133 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/conversationTimestamp.py
--rw-r--r--   0        0        0     1303 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createConversationPayload.py
--rw-r--r--   0        0        0     1522 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createConversationResponse.py
--rw-r--r--   0        0        0     1428 2023-04-11 15:54:47.939454 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createUserPayload.py
--rw-r--r--   0        0        0     1399 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/deleteMemberPayload.py
--rw-r--r--   0        0        0     1501 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/earmuffPayload.py
--rw-r--r--   0        0        0     1073 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/earmuffResponseBody.py
--rw-r--r--   0        0        0     1152 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/embeddedUsers.py
--rw-r--r--   0        0        0     1229 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/eventEmbedded.py
--rw-r--r--   0        0        0     1396 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/eventResponse.py
--rw-r--r--   0        0        0     1271 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/getUsersResponse.py
--rw-r--r--   0        0        0     1751 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/inviteMemberPayload.py
--rw-r--r--   0        0        0     1121 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/leg.py
--rw-r--r--   0        0        0     1315 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/media.py
--rw-r--r--   0        0        0     1063 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/member.py
--rw-r--r--   0        0        0     1570 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/memberResponse.py
--rw-r--r--   0        0        0     1121 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/memberTimestamp.py
--rw-r--r--   0        0        0     1483 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/mutePayload.py
--rw-r--r--   0        0        0     1070 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/muteResponseBody.py
--rw-r--r--   0        0        0     1571 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/onInboundCallPayload.py
--rw-r--r--   0        0        0     1187 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStopBody.py
--rw-r--r--   0        0        0     1572 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStopPayload.py
--rw-r--r--   0        0        0     1226 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamBody.py
--rw-r--r--   0        0        0     1490 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamPayload.py
--rw-r--r--   0        0        0     1155 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamResponseBody.py
--rw-r--r--   0        0        0     1081 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamStopResponseBody.py
--rw-r--r--   0        0        0     1197 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/reason.py
--rw-r--r--   0        0        0     1122 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/responseProperties.py
--rw-r--r--   0        0        0     1179 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayStopBody.py
--rw-r--r--   0        0        0     1559 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayStopPayload.py
--rw-r--r--   0        0        0     1313 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextBody.py
--rw-r--r--   0        0        0     1321 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextParams.py
--rw-r--r--   0        0        0     1468 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextPayload.py
--rw-r--r--   0        0        0     1126 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/selfLink.py
--rw-r--r--   0        0        0     1966 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/transferMemberPayload.py
--rw-r--r--   0        0        0     1456 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/updateUserPayload.py
--rw-r--r--   0        0        0     1235 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/user.py
--rw-r--r--   0        0        0     1123 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userEmbedded.py
--rw-r--r--   0        0        0     1453 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userResponse.py
--rw-r--r--   0        0        0     1184 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userSummary.py
--rw-r--r--   0        0        0     1125 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userTimestamp.py
--rw-r--r--   0        0        0     1294 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiAnswerCallBack.py
--rw-r--r--   0        0        0     1301 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallOptions.py
--rw-r--r--   0        0        0     2231 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallPayload.py
--rw-r--r--   0        0        0     1136 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallResponse.py
--rw-r--r--   0        0        0     1338 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiEventCallBackPayload.py
--rw-r--r--   0        0        0     1227 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiEventParams.py
--rw-r--r--   0        0        0    11681 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/conversation.py
--rw-r--r--   0        0        0      253 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/csChannelTypes.py
--rw-r--r--   0        0        0      743 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/csEvents.py
--rw-r--r--   0        0        0      174 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/memberActions.py
--rw-r--r--   0        0        0      243 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/memberStates.py
--rw-r--r--   0        0        0     3730 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/users.py
--rw-r--r--   0        0        0     7104 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/voice.py
--rw-r--r--   0        0        0      405 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/voice/voiceActions.py
--rw-r--r--   0        0        0      414 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/IVonageAI.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/__init__.py
--rw-r--r--   0        0        0      193 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/IImportPayload.py
--rw-r--r--   0        0        0      288 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/IVonageAiAnalyzePayload.py
--rw-r--r--   0        0        0      384 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/IVonageAiImportModelPayload.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/importPayload.py
--rw-r--r--   0        0        0     1369 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/vonageAiAnalyzePayload.py
--rw-r--r--   0        0        0     1489 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/vonageAiImportModelPayload.py
--rw-r--r--   0        0        0     2513 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/vonageAI.py
--rw-r--r--   0        0        0      209 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/vonageAIActions.py
--rw-r--r--   0        0        0      385 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/IVonageAPI.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/__init__.py
--rw-r--r--   0        0        0      241 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/contracts/IInvokePayload.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/contracts/__init__.py
--rw-r--r--   0        0        0     1304 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/contracts/invokePayload.py
--rw-r--r--   0        0        0     1775 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/vonageAPI.py
--rw-r--r--   0        0        0      181 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/vonageAPIActions.py
--rw-r--r--   0        0        0      222 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/IFormDataObject.py
--rw-r--r--   0        0        0      194 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/IRequest.py
--rw-r--r--   0        0        0      356 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/IRequestParams.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/__init__.py
--rw-r--r--   0        0        0     1181 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/formDataObject.py
--rw-r--r--   0        0        0     1130 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/request.py
--rw-r--r--   0        0        0      288 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/requestMethods.py
--rw-r--r--   0        0        0     1335 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/requestParams.py
--rw-r--r--   0        0        0      264 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/request/responseTypes.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/__init__.py
--rw-r--r--   0        0        0      276 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/commandService/ICommandService.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/commandService/__init__.py
--rw-r--r--   0        0        0     1697 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/commandService/commandService.py
--rw-r--r--   0        0        0      551 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/IConfig.py
--rw-r--r--   0        0        0      234 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/IPathObject.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/__init__.py
--rw-r--r--   0        0        0     4016 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/config.py
--rw-r--r--   0        0        0     1191 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/config/pathObject.py
--rw-r--r--   0        0        0      201 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/IAcl.py
--rw-r--r--   0        0        0      242 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/ICreateVonageTokenParams.py
--rw-r--r--   0        0        0      437 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/IJwt.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/__init__.py
--rw-r--r--   0        0        0     1130 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/acl.py
--rw-r--r--   0        0        0     1247 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/createVonageTokenParams.py
--rw-r--r--   0        0        0     3103 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/jwt.py
--rw-r--r--   0        0        0     1224 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/neruJWTPayload.py
--rw-r--r--   0        0        0     1203 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/services/jwt/vonageJWTPayload.py
--rw-r--r--   0        0        0      405 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IActionPayload.py
--rw-r--r--   0        0        0      318 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/ICommand.py
--rw-r--r--   0        0        0      212 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IFilter.py
--rw-r--r--   0        0        0      274 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IPayloadWithCallback.py
--rw-r--r--   0        0        0      281 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IRequestInterface.py
--rw-r--r--   0        0        0     1203 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/ISession.py
--rw-r--r--   0        0        0      337 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/IWrappedCallback.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/__init__.py
--rw-r--r--   0        0        0     1601 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/actionPayload.py
--rw-r--r--   0        0        0     1324 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/command.py
--rw-r--r--   0        0        0     1229 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/filter.py
--rw-r--r--   0        0        0     5721 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/neruSession.py
--rw-r--r--   0        0        0     1280 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/payloadWithCallback.py
--rw-r--r--   0        0        0     1827 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/requestInterface.py
--rw-r--r--   0        0        0     1665 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/requestInterfaceForCallbacks.py
--rw-r--r--   0        0        0     1541 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/requestInterfaceWithParams.py
--rw-r--r--   0        0        0     1302 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/session/wrappedCallback.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/__init__.py
--rw-r--r--   0        0        0     2180 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/assetsTest.py
--rw-r--r--   0        0        0     4230 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/messagesTest.py
--rw-r--r--   0        0        0     3884 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/schedulerTest.py
--rw-r--r--   0        0        0     1106 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/schedulerTestPayload.py
--rw-r--r--   0        0        0     2734 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/stateTest.py
--rw-r--r--   0        0        0     3983 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/smokes/voiceTest.py
--rw-r--r--   0        0        0      250 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/IBaseEvent.py
--rw-r--r--   0        0        0      183 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/IUrlPayload.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/__init__.py
--rw-r--r--   0        0        0     1202 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/baseEvent.py
--rw-r--r--   0        0        0      261 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessangerEvent.py
--rw-r--r--   0        0        0      352 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerAudioEvent.py
--rw-r--r--   0        0        0      350 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerFileEvent.py
--rw-r--r--   0        0        0      352 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerImageEvent.py
--rw-r--r--   0        0        0      282 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerTextEvent.py
--rw-r--r--   0        0        0      285 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerUnsupportedEvent.py
--rw-r--r--   0        0        0      352 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/IMessengerVideoEvent.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/__init__.py
--rw-r--r--   0        0        0     1357 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerAudioEvent.py
--rw-r--r--   0        0        0     1254 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerEvent.py
--rw-r--r--   0        0        0     1352 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerFileEvent.py
--rw-r--r--   0        0        0     1357 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerImageEvent.py
--rw-r--r--   0        0        0     1284 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerTextEvent.py
--rw-r--r--   0        0        0     1298 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerUnsupportedEvent.py
--rw-r--r--   0        0        0     1357 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerVideoEvent.py
--rw-r--r--   0        0        0      322 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSAudioEvent.py
--rw-r--r--   0        0        0      255 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSEvent.py
--rw-r--r--   0        0        0      322 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSImageEvent.py
--rw-r--r--   0        0        0      322 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSVCardEvent.py
--rw-r--r--   0        0        0      322 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/IMMSVideoEvent.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/__init__.py
--rw-r--r--   0        0        0     1327 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsAudioEvent.py
--rw-r--r--   0        0        0     1224 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsEvent.py
--rw-r--r--   0        0        0     1327 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsImageEvent.py
--rw-r--r--   0        0        0     1327 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsVCardEvent.py
--rw-r--r--   0        0        0     1327 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsVideoEvent.py
--rw-r--r--   0        0        0      417 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/ISMSEvent.py
--rw-r--r--   0        0        0      209 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/ISMSMetadata.py
--rw-r--r--   0        0        0      200 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/ISMSUsage.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/__init__.py
--rw-r--r--   0        0        0     1385 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsEvent.py
--rw-r--r--   0        0        0     1168 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsMetadata.py
--rw-r--r--   0        0        0     1150 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsUsage.py
--rw-r--r--   0        0        0     1134 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/urlPayload.py
--rw-r--r--   0        0        0      270 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/viber/IViberEvent.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.943455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/viber/__init__.py
--rw-r--r--   0        0        0     1248 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/viber/viberEvent.py
--rw-r--r--   0        0        0      328 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/webhookEventTypes.py
--rw-r--r--   0        0        0      222 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IMessageEventContext.py
--rw-r--r--   0        0        0      185 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IProfileName.py
--rw-r--r--   0        0        0      217 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IReplyObject.py
--rw-r--r--   0        0        0      347 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappAudioEvent.py
--rw-r--r--   0        0        0      501 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappEvent.py
--rw-r--r--   0        0        0      345 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappFileEvent.py
--rw-r--r--   0        0        0      347 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappImageEvent.py
--rw-r--r--   0        0        0      359 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappReplyEvent.py
--rw-r--r--   0        0        0      277 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappTextEvent.py
--rw-r--r--   0        0        0      280 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappUnsupportedEvent.py
--rw-r--r--   0        0        0      347 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/IWhatsappVideoEvent.py
--rw-r--r--   0        0        0        0 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/messageEventContext.py
--rw-r--r--   0        0        0     1148 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/profileName.py
--rw-r--r--   0        0        0     1189 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/replyObject.py
--rw-r--r--   0        0        0     1617 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappAudioEvent.py
--rw-r--r--   0        0        0     1612 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappFileEvent.py
--rw-r--r--   0        0        0     1617 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappImageEvent.py
--rw-r--r--   0        0        0     1629 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappReplyEvent.py
--rw-r--r--   0        0        0     1544 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappTextEvent.py
--rw-r--r--   0        0        0     1558 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappUnsupportedEvent.py
--rw-r--r--   0        0        0     1617 2023-04-11 15:54:47.947455 nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappVideoEvent.py
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 nerualpha-4.1.0rc5/PKG-INFO
+-rw-r--r--   0        0        0      594 2023-05-30 13:25:38.319589 nerualpha-5.0.0/README.md
+-rw-r--r--   0        0        0      837 2023-05-30 13:25:38.319589 nerualpha-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1912 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/IBridge.py
+-rw-r--r--   0        0        0      878 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/INeru.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/__init__.py
+-rw-r--r--   0        0        0     4323 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/bridge.py
+-rw-r--r--   0        0        0     3977 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/neru.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/__init__.py
+-rw-r--r--   0        0        0     1459 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/IAssets.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/__init__.py
+-rw-r--r--   0        0        0     6108 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/assets.py
+-rw-r--r--   0        0        0      316 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/assetsActions.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/__init__.py
+-rw-r--r--   0        0        0     1112 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/assetInfo.py
+-rw-r--r--   0        0        0     1083 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/assetLinkResponse.py
+-rw-r--r--   0        0        0     1149 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/assetListResponse.py
+-rw-r--r--   0        0        0     1105 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/directoryPayload.py
+-rw-r--r--   0        0        0     1092 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/getAssetPayload.py
+-rw-r--r--   0        0        0     1098 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/getAssetResponse.py
+-rw-r--r--   0        0        0     1155 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/linkPayload.py
+-rw-r--r--   0        0        0     1228 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/listAssetsPayload.py
+-rw-r--r--   0        0        0     1176 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/removeAssetPayload.py
+-rw-r--r--   0        0        0      334 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/assets/fileRetentionPeriod.py
+-rw-r--r--   0        0        0      328 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/IEventEmitter.py
+-rw-r--r--   0        0        0      336 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/IEventFactory.py
+-rw-r--r--   0        0        0      404 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/INeruEvent.py
+-rw-r--r--   0        0        0      200 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/ISessionCreatedDetails.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/__init__.py
+-rw-r--r--   0        0        0     2838 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/eventEmitter.py
+-rw-r--r--   0        0        0     2438 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/eventFactory.py
+-rw-r--r--   0        0        0     1364 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/neruEvent.py
+-rw-r--r--   0        0        0      189 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/neruEventSourceTypes.py
+-rw-r--r--   0        0        0      477 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/neruEventTypes.py
+-rw-r--r--   0        0        0     1229 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/events/sessionCreatedDetails.py
+-rw-r--r--   0        0        0      447 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/logger/ILogAction.py
+-rw-r--r--   0        0        0      221 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/logger/ILogContext.py
+-rw-r--r--   0        0        0      334 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/logger/ILogger.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/logger/__init__.py
+-rw-r--r--   0        0        0     1415 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/logger/logAction.py
+-rw-r--r--   0        0        0     1307 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/logger/logContext.py
+-rw-r--r--   0        0        0      228 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/logger/logLevels.py
+-rw-r--r--   0        0        0     3046 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/logger/logger.py
+-rw-r--r--   0        0        0      212 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/logger/sourceTypes.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/__init__.py
+-rw-r--r--   0        0        0      199 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/ICreateRoomPayload.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/__init__.py
+-rw-r--r--   0        0        0     1698 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/createRoomPayload.py
+-rw-r--r--   0        0        0     1055 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/deleteRoomPayload.py
+-rw-r--r--   0        0        0     1274 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/getRoomsResponse.py
+-rw-r--r--   0        0        0     1194 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/pageLinks.py
+-rw-r--r--   0        0        0     1111 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/recordingOptions.py
+-rw-r--r--   0        0        0     1158 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/roomLinks.py
+-rw-r--r--   0        0        0     1465 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/roomResponse.py
+-rw-r--r--   0        0        0     1158 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/roomsEmbedded.py
+-rw-r--r--   0        0        0     1219 2023-05-30 13:25:38.319589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/updateRoomDetails.py
+-rw-r--r--   0        0        0     1251 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/updateRoomPayload.py
+-rw-r--r--   0        0        0     3349 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/meetings/meetings.py
+-rw-r--r--   0        0        0      203 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/meetings/roomTypes.py
+-rw-r--r--   0        0        0     1863 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/IMessages.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/__init__.py
+-rw-r--r--   0        0        0      234 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IBaseMessage.py
+-rw-r--r--   0        0        0      198 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IImageData.py
+-rw-r--r--   0        0        0      495 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IListenEventsPayload.py
+-rw-r--r--   0        0        0      497 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IListenMessagesPayload.py
+-rw-r--r--   0        0        0      359 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMMSAudioMessage.py
+-rw-r--r--   0        0        0      359 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMMSImageMessage.py
+-rw-r--r--   0        0        0      359 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMMSVCardMessage.py
+-rw-r--r--   0        0        0      359 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMMSVideoMessage.py
+-rw-r--r--   0        0        0      215 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMessageContact.py
+-rw-r--r--   0        0        0      199 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMessenger.py
+-rw-r--r--   0        0        0      365 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMessengerAudioMessage.py
+-rw-r--r--   0        0        0      363 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMessengerFileMessage.py
+-rw-r--r--   0        0        0      365 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMessengerImageMessage.py
+-rw-r--r--   0        0        0      194 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMessengerTextMessage.py
+-rw-r--r--   0        0        0      365 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IMessengerVideoMessage.py
+-rw-r--r--   0        0        0      270 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/ISMSMessage.py
+-rw-r--r--   0        0        0      285 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/ISendImageContent.py
+-rw-r--r--   0        0        0      294 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/ISendImageMessage.py
+-rw-r--r--   0        0        0      426 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/ISendImagePayload.py
+-rw-r--r--   0        0        0      276 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/ISendImageResponse.py
+-rw-r--r--   0        0        0      194 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/ISendResponse.py
+-rw-r--r--   0        0        0      203 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/ISendTextContent.py
+-rw-r--r--   0        0        0      297 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/ISendTextMessagePayload.py
+-rw-r--r--   0        0        0      443 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/ISendTextPayload.py
+-rw-r--r--   0        0        0      199 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IURLPayload.py
+-rw-r--r--   0        0        0      196 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IUnsubscribeEventsPayload.py
+-rw-r--r--   0        0        0      361 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IViberImageMessage.py
+-rw-r--r--   0        0        0      216 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IViberService.py
+-rw-r--r--   0        0        0      276 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IViberTextMessage.py
+-rw-r--r--   0        0        0      199 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IWhatsapp.py
+-rw-r--r--   0        0        0      364 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IWhatsappAudioMessage.py
+-rw-r--r--   0        0        0      362 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IWhatsappFileMessage.py
+-rw-r--r--   0        0        0      364 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IWhatsappImageMessage.py
+-rw-r--r--   0        0        0      215 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IWhatsappTemplate.py
+-rw-r--r--   0        0        0      482 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IWhatsappTemplateMessage.py
+-rw-r--r--   0        0        0      279 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IWhatsappTextMessage.py
+-rw-r--r--   0        0        0      364 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/IWhatsappVideoMessage.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/__init__.py
+-rw-r--r--   0        0        0     1206 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/baseMessage.py
+-rw-r--r--   0        0        0     1230 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/imageData.py
+-rw-r--r--   0        0        0     1544 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/listenEventsPayload.py
+-rw-r--r--   0        0        0     1552 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/listenMessagesPayload.py
+-rw-r--r--   0        0        0     1202 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messageContact.py
+-rw-r--r--   0        0        0     1508 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerAudioMessage.py
+-rw-r--r--   0        0        0     1502 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerFileMessage.py
+-rw-r--r--   0        0        0     1508 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerImageMessage.py
+-rw-r--r--   0        0        0     1419 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerTextMessage.py
+-rw-r--r--   0        0        0     1508 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerVideoMessage.py
+-rw-r--r--   0        0        0     1385 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/mmsAudioMessage.py
+-rw-r--r--   0        0        0     1372 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/mmsImageMessage.py
+-rw-r--r--   0        0        0     1372 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/mmsVCardMessage.py
+-rw-r--r--   0        0        0     1372 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/mmsVideoMessage.py
+-rw-r--r--   0        0        0     1342 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendImageContent.py
+-rw-r--r--   0        0        0     1328 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendImageMessage.py
+-rw-r--r--   0        0        0     1731 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendImagePayload.py
+-rw-r--r--   0        0        0     1166 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendResponse.py
+-rw-r--r--   0        0        0     1240 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendTextContent.py
+-rw-r--r--   0        0        0     1348 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendTextMessagePayload.py
+-rw-r--r--   0        0        0     1768 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendTextPayload.py
+-rw-r--r--   0        0        0     1267 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/smsMessage.py
+-rw-r--r--   0        0        0     1225 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/unsubscribeEventsPayload.py
+-rw-r--r--   0        0        0     1173 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/urlPayload.py
+-rw-r--r--   0        0        0     1509 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/viberImageMessage.py
+-rw-r--r--   0        0        0     1420 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/viberTextMessage.py
+-rw-r--r--   0        0        0     1397 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappAudioMessage.py
+-rw-r--r--   0        0        0     1391 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappFileMessage.py
+-rw-r--r--   0        0        0     1397 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappImageMessage.py
+-rw-r--r--   0        0        0     1528 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappTemplateMessage.py
+-rw-r--r--   0        0        0     1308 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappTextMessage.py
+-rw-r--r--   0        0        0     1397 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappVideoMessage.py
+-rw-r--r--   0        0        0      317 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/messageActions.py
+-rw-r--r--   0        0        0      219 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/messageChannelType.py
+-rw-r--r--   0        0        0      298 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/messageType.py
+-rw-r--r--   0        0        0     5175 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/messages/messages.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/__init__.py
+-rw-r--r--   0        0        0      187 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/IBaseNumberOptions.py
+-rw-r--r--   0        0        0      411 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/IGetNumbersOptions.py
+-rw-r--r--   0        0        0      331 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/INumberOptions.py
+-rw-r--r--   0        0        0      403 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/ISearchNumbersOptions.py
+-rw-r--r--   0        0        0      450 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/IUpdateNumberOptions.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/baseNumberOptions.py
+-rw-r--r--   0        0        0     1453 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/getNumbersOptions.py
+-rw-r--r--   0        0        0     1185 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/getNumbersResponse.py
+-rw-r--r--   0        0        0     1315 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/numberOptions.py
+-rw-r--r--   0        0        0     1259 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/numberResponse.py
+-rw-r--r--   0        0        0     1129 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/numbersOperationResponse.py
+-rw-r--r--   0        0        0     1515 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/searchNumbersOptions.py
+-rw-r--r--   0        0        0     1492 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/updateNumberOptions.py
+-rw-r--r--   0        0        0      208 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/numberFeature.py
+-rw-r--r--   0        0        0     7877 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/numbers/numbers.py
+-rw-r--r--   0        0        0     1802 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/IQueue.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/ICreateQueueOptions.py
+-rw-r--r--   0        0        0      392 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/ICreateQueuePayload.py
+-rw-r--r--   0        0        0      386 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/IQueueDetails.py
+-rw-r--r--   0        0        0      280 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/IQueueDetailsStats.py
+-rw-r--r--   0        0        0      211 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/IQueueRate.py
+-rw-r--r--   0        0        0      220 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/IUpdateQueueOptions.py
+-rw-r--r--   0        0        0      269 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/IUpdateQueuePayload.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/__init__.py
+-rw-r--r--   0        0        0     1225 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/createQueueOptions.py
+-rw-r--r--   0        0        0     1382 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/createQueuePayload.py
+-rw-r--r--   0        0        0      402 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/queueDetailsResponse.py
+-rw-r--r--   0        0        0     1172 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/queueRate.py
+-rw-r--r--   0        0        0     1208 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/updateQueueOptions.py
+-rw-r--r--   0        0        0     1256 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/updateQueuePayload.py
+-rw-r--r--   0        0        0     7099 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/queue/queue.py
+-rw-r--r--   0        0        0     1099 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/IScheduler.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/__init__.py
+-rw-r--r--   0        0        0      289 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/IIntervalParams.py
+-rw-r--r--   0        0        0      208 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/IListAllPayload.py
+-rw-r--r--   0        0        0      187 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/ISchedulePayload.py
+-rw-r--r--   0        0        0      390 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/IStartAtParams.py
+-rw-r--r--   0        0        0      463 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/IStartAtPayload.py
+-rw-r--r--   0        0        0      208 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/IUntilParams.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/__init__.py
+-rw-r--r--   0        0        0     1381 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/getSchedulerResponse.py
+-rw-r--r--   0        0        0     1269 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/intervalParams.py
+-rw-r--r--   0        0        0     1315 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/listAllPayload.py
+-rw-r--r--   0        0        0     1123 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/listAllSchedulersResponse.py
+-rw-r--r--   0        0        0     1138 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/schedulerExecutionInfo.py
+-rw-r--r--   0        0        0     1191 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/schedulerPayload.py
+-rw-r--r--   0        0        0     1391 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/startAtParams.py
+-rw-r--r--   0        0        0     1472 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/startAtPayload.py
+-rw-r--r--   0        0        0     1179 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/untilParams.py
+-rw-r--r--   0        0        0     4064 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/scheduler.py
+-rw-r--r--   0        0        0      237 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/scheduler/schedulerActions.py
+-rw-r--r--   0        0        0     2277 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/state/IState.py
+-rw-r--r--   0        0        0      240 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/state/IStateCommand.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/state/__init__.py
+-rw-r--r--   0        0        0      212 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/state/expireOptions.py
+-rw-r--r--   0        0        0    10251 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/state/state.py
+-rw-r--r--   0        0        0     1367 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/state/stateCommand.py
+-rw-r--r--   0        0        0      694 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/state/stateOperations.py
+-rw-r--r--   0        0        0     4626 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/IConversation.py
+-rw-r--r--   0        0        0     1278 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/IUsers.py
+-rw-r--r--   0        0        0     1864 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/IVoice.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/callDirections.py
+-rw-r--r--   0        0        0      257 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/callStatuses.py
+-rw-r--r--   0        0        0      344 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IAcceptInboundCallBody.py
+-rw-r--r--   0        0        0      215 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IAcceptInboundCallEndpoint.py
+-rw-r--r--   0        0        0      403 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IAcceptInboundCallEvent.py
+-rw-r--r--   0        0        0      460 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IAcceptInboundCallPayload.py
+-rw-r--r--   0        0        0      209 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IAddUserPayload.py
+-rw-r--r--   0        0        0      225 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IAudioSettings.py
+-rw-r--r--   0        0        0      536 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IChannel.py
+-rw-r--r--   0        0        0      190 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IChannelEndpoint.py
+-rw-r--r--   0        0        0      291 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IChannelPhoneEndpoint.py
+-rw-r--r--   0        0        0      346 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IChannelSIPEndpoint.py
+-rw-r--r--   0        0        0      292 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IChannelVBCEndpoint.py
+-rw-r--r--   0        0        0      304 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IConversationPayloadWithCallback.py
+-rw-r--r--   0        0        0      220 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/ICreateConversationPayload.py
+-rw-r--r--   0        0        0      250 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/ICreateUserPayload.py
+-rw-r--r--   0        0        0      277 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IDeleteMemberPayload.py
+-rw-r--r--   0        0        0      214 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IEarmuffPayload.py
+-rw-r--r--   0        0        0      371 2023-05-30 13:25:38.323589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IInviteMemberPayload.py
+-rw-r--r--   0        0        0      179 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/ILeg.py
+-rw-r--r--   0        0        0      293 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IMedia.py
+-rw-r--r--   0        0        0      211 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IMutePayload.py
+-rw-r--r--   0        0        0      423 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IOnInboundCallPayload.py
+-rw-r--r--   0        0        0      189 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IPlayStopBody.py
+-rw-r--r--   0        0        0      300 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IPlayStopPayload.py
+-rw-r--r--   0        0        0      241 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IPlayStreamBody.py
+-rw-r--r--   0        0        0      308 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IPlayStreamPayload.py
+-rw-r--r--   0        0        0      193 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IReason.py
+-rw-r--r--   0        0        0      187 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/ISayStopBody.py
+-rw-r--r--   0        0        0      296 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/ISayStopPayload.py
+-rw-r--r--   0        0        0      291 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/ISayTextBody.py
+-rw-r--r--   0        0        0      293 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/ISayTextParams.py
+-rw-r--r--   0        0        0      285 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/ISayTextPayload.py
+-rw-r--r--   0        0        0      373 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/ITransferMemberPayload.py
+-rw-r--r--   0        0        0      250 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IUpdateUserPayload.py
+-rw-r--r--   0        0        0      251 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IUser.py
+-rw-r--r--   0        0        0      277 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IVapiAnswerCallBack.py
+-rw-r--r--   0        0        0      274 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IVapiCreateCallOptions.py
+-rw-r--r--   0        0        0      373 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IVapiCreateCallPayload.py
+-rw-r--r--   0        0        0      312 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IVapiEventCallBackPayload.py
+-rw-r--r--   0        0        0      233 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IVapiEventParams.py
+-rw-r--r--   0        0        0     1063 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/Link.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/__init__.py
+-rw-r--r--   0        0        0     1341 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/acceptInboundCallBody.py
+-rw-r--r--   0        0        0     1224 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/acceptInboundCallEndpoint.py
+-rw-r--r--   0        0        0     1407 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/acceptInboundCallEvent.py
+-rw-r--r--   0        0        0     1852 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/acceptInboundCallPayload.py
+-rw-r--r--   0        0        0     1245 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/addUserPayload.py
+-rw-r--r--   0        0        0     1351 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/addUserResponse.py
+-rw-r--r--   0        0        0     1261 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/audioSayResponseBody.py
+-rw-r--r--   0        0        0     1078 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/audioSayStopResponseBody.py
+-rw-r--r--   0        0        0     1326 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/audioSettings.py
+-rw-r--r--   0        0        0     1605 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channel.py
+-rw-r--r--   0        0        0     1320 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channelAppEndpoint.py
+-rw-r--r--   0        0        0     1347 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channelPhoneEndpoint.py
+-rw-r--r--   0        0        0     1656 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channelSIPEndpoint.py
+-rw-r--r--   0        0        0     1349 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channelVBCEndpoint.py
+-rw-r--r--   0        0        0     1453 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/conversationPayloadWithCallback.py
+-rw-r--r--   0        0        0     1133 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/conversationTimestamp.py
+-rw-r--r--   0        0        0     1313 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/createConversationPayload.py
+-rw-r--r--   0        0        0     1522 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/createConversationResponse.py
+-rw-r--r--   0        0        0     1451 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/createUserPayload.py
+-rw-r--r--   0        0        0     1408 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/deleteMemberPayload.py
+-rw-r--r--   0        0        0     1517 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/earmuffPayload.py
+-rw-r--r--   0        0        0     1073 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/earmuffResponseBody.py
+-rw-r--r--   0        0        0     1152 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/embeddedUsers.py
+-rw-r--r--   0        0        0     1229 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/eventEmbedded.py
+-rw-r--r--   0        0        0     1412 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/eventResponse.py
+-rw-r--r--   0        0        0     1271 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/getUsersResponse.py
+-rw-r--r--   0        0        0     1766 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/inviteMemberPayload.py
+-rw-r--r--   0        0        0     1121 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/leg.py
+-rw-r--r--   0        0        0     1337 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/media.py
+-rw-r--r--   0        0        0     1063 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/member.py
+-rw-r--r--   0        0        0     1570 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/memberResponse.py
+-rw-r--r--   0        0        0     1121 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/memberTimestamp.py
+-rw-r--r--   0        0        0     1499 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/mutePayload.py
+-rw-r--r--   0        0        0     1070 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/muteResponseBody.py
+-rw-r--r--   0        0        0     1635 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/onInboundCallPayload.py
+-rw-r--r--   0        0        0     1192 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStopBody.py
+-rw-r--r--   0        0        0     1582 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStopPayload.py
+-rw-r--r--   0        0        0     1226 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStreamBody.py
+-rw-r--r--   0        0        0     1512 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStreamPayload.py
+-rw-r--r--   0        0        0     1155 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStreamResponseBody.py
+-rw-r--r--   0        0        0     1081 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStreamStopResponseBody.py
+-rw-r--r--   0        0        0     1207 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/reason.py
+-rw-r--r--   0        0        0     1122 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/responseProperties.py
+-rw-r--r--   0        0        0     1184 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayStopBody.py
+-rw-r--r--   0        0        0     1569 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayStopPayload.py
+-rw-r--r--   0        0        0     1313 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayTextBody.py
+-rw-r--r--   0        0        0     1321 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayTextParams.py
+-rw-r--r--   0        0        0     1487 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayTextPayload.py
+-rw-r--r--   0        0        0     1126 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/selfLink.py
+-rw-r--r--   0        0        0     1976 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/transferMemberPayload.py
+-rw-r--r--   0        0        0     1479 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/updateUserPayload.py
+-rw-r--r--   0        0        0     1235 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/user.py
+-rw-r--r--   0        0        0     1123 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/userEmbedded.py
+-rw-r--r--   0        0        0     1453 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/userResponse.py
+-rw-r--r--   0        0        0     1184 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/userSummary.py
+-rw-r--r--   0        0        0     1125 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/userTimestamp.py
+-rw-r--r--   0        0        0     1312 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiAnswerCallBack.py
+-rw-r--r--   0        0        0     1301 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiCreateCallOptions.py
+-rw-r--r--   0        0        0     2331 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiCreateCallPayload.py
+-rw-r--r--   0        0        0     1136 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiCreateCallResponse.py
+-rw-r--r--   0        0        0     1338 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiEventCallBackPayload.py
+-rw-r--r--   0        0        0     1227 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiEventParams.py
+-rw-r--r--   0        0        0    11984 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/conversation.py
+-rw-r--r--   0        0        0      253 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/csChannelTypes.py
+-rw-r--r--   0        0        0      743 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/csEvents.py
+-rw-r--r--   0        0        0      174 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/memberActions.py
+-rw-r--r--   0        0        0      243 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/memberStates.py
+-rw-r--r--   0        0        0     3837 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/users.py
+-rw-r--r--   0        0        0     7347 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/voice.py
+-rw-r--r--   0        0        0      405 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/voice/voiceActions.py
+-rw-r--r--   0        0        0      434 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/IVonageAI.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/IImportPayload.py
+-rw-r--r--   0        0        0      288 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/IVonageAiAnalyzePayload.py
+-rw-r--r--   0        0        0      384 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/IVonageAiImportModelPayload.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/__init__.py
+-rw-r--r--   0        0        0     1213 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/importPayload.py
+-rw-r--r--   0        0        0     1392 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/vonageAiAnalyzePayload.py
+-rw-r--r--   0        0        0     1523 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/vonageAiImportModelPayload.py
+-rw-r--r--   0        0        0     2543 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/vonageAI.py
+-rw-r--r--   0        0        0      209 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAI/vonageAIActions.py
+-rw-r--r--   0        0        0      431 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAPI/IVonageAPI.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAPI/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAPI/contracts/IInvokePayload.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAPI/contracts/__init__.py
+-rw-r--r--   0        0        0     1333 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAPI/contracts/invokePayload.py
+-rw-r--r--   0        0        0     1831 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAPI/vonageAPI.py
+-rw-r--r--   0        0        0      181 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/providers/vonageAPI/vonageAPIActions.py
+-rw-r--r--   0        0        0      222 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/request/IFormDataObject.py
+-rw-r--r--   0        0        0      194 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/request/IRequest.py
+-rw-r--r--   0        0        0      372 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/request/IRequestParams.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/request/__init__.py
+-rw-r--r--   0        0        0     1181 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/request/formDataObject.py
+-rw-r--r--   0        0        0     1130 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/request/request.py
+-rw-r--r--   0        0        0      288 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/request/requestMethods.py
+-rw-r--r--   0        0        0     1351 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/request/requestParams.py
+-rw-r--r--   0        0        0      264 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/request/responseTypes.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/commandService/ICommandService.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/commandService/__init__.py
+-rw-r--r--   0        0        0     1767 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/commandService/commandService.py
+-rw-r--r--   0        0        0      576 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/config/IConfig.py
+-rw-r--r--   0        0        0      234 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/config/IPathObject.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/config/__init__.py
+-rw-r--r--   0        0        0     4115 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/config/config.py
+-rw-r--r--   0        0        0     1191 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/config/pathObject.py
+-rw-r--r--   0        0        0      201 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/jwt/IAcl.py
+-rw-r--r--   0        0        0      242 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/jwt/ICreateVonageTokenParams.py
+-rw-r--r--   0        0        0      463 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/jwt/IJwt.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/jwt/__init__.py
+-rw-r--r--   0        0        0     1130 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/jwt/acl.py
+-rw-r--r--   0        0        0     1247 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/jwt/createVonageTokenParams.py
+-rw-r--r--   0        0        0     3152 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/jwt/jwt.py
+-rw-r--r--   0        0        0     1224 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/jwt/neruJWTPayload.py
+-rw-r--r--   0        0        0     1203 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/services/jwt/vonageJWTPayload.py
+-rw-r--r--   0        0        0      421 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/IActionPayload.py
+-rw-r--r--   0        0        0      334 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/ICommand.py
+-rw-r--r--   0        0        0      212 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/IFilter.py
+-rw-r--r--   0        0        0      274 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/IPayloadWithCallback.py
+-rw-r--r--   0        0        0      314 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/IRequestInterface.py
+-rw-r--r--   0        0        0     1303 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/ISession.py
+-rw-r--r--   0        0        0      337 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/IWrappedCallback.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/__init__.py
+-rw-r--r--   0        0        0     1635 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/actionPayload.py
+-rw-r--r--   0        0        0     1374 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/command.py
+-rw-r--r--   0        0        0     1250 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/filter.py
+-rw-r--r--   0        0        0     5872 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/neruSession.py
+-rw-r--r--   0        0        0     1298 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/payloadWithCallback.py
+-rw-r--r--   0        0        0     1904 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/requestInterface.py
+-rw-r--r--   0        0        0     1734 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/requestInterfaceForCallbacks.py
+-rw-r--r--   0        0        0     1603 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/requestInterfaceWithParams.py
+-rw-r--r--   0        0        0     1302 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/session/wrappedCallback.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/smokes/__init__.py
+-rw-r--r--   0        0        0     2195 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/smokes/assetsTest.py
+-rw-r--r--   0        0        0     4305 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/smokes/messagesTest.py
+-rw-r--r--   0        0        0     3914 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/smokes/schedulerTest.py
+-rw-r--r--   0        0        0     1106 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/smokes/schedulerTestPayload.py
+-rw-r--r--   0        0        0     2744 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/smokes/stateTest.py
+-rw-r--r--   0        0        0     4043 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/smokes/voiceTest.py
+-rw-r--r--   0        0        0      250 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/webhookEvents/IBaseEvent.py
+-rw-r--r--   0        0        0      183 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/webhookEvents/IUrlPayload.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/webhookEvents/__init__.py
+-rw-r--r--   0        0        0     1202 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/webhookEvents/baseEvent.py
+-rw-r--r--   0        0        0      261 2023-05-30 13:25:38.327589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/IMessangerEvent.py
+-rw-r--r--   0        0        0      352 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/IMessengerAudioEvent.py
+-rw-r--r--   0        0        0      350 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/IMessengerFileEvent.py
+-rw-r--r--   0        0        0      352 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/IMessengerImageEvent.py
+-rw-r--r--   0        0        0      282 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/IMessengerTextEvent.py
+-rw-r--r--   0        0        0      285 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/IMessengerUnsupportedEvent.py
+-rw-r--r--   0        0        0      352 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/IMessengerVideoEvent.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerAudioEvent.py
+-rw-r--r--   0        0        0     1254 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerEvent.py
+-rw-r--r--   0        0        0     1352 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerFileEvent.py
+-rw-r--r--   0        0        0     1357 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerImageEvent.py
+-rw-r--r--   0        0        0     1284 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerTextEvent.py
+-rw-r--r--   0        0        0     1298 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerUnsupportedEvent.py
+-rw-r--r--   0        0        0     1357 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerVideoEvent.py
+-rw-r--r--   0        0        0      322 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/IMMSAudioEvent.py
+-rw-r--r--   0        0        0      255 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/IMMSEvent.py
+-rw-r--r--   0        0        0      322 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/IMMSImageEvent.py
+-rw-r--r--   0        0        0      322 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/IMMSVCardEvent.py
+-rw-r--r--   0        0        0      322 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/IMMSVideoEvent.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/__init__.py
+-rw-r--r--   0        0        0     1327 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsAudioEvent.py
+-rw-r--r--   0        0        0     1224 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsEvent.py
+-rw-r--r--   0        0        0     1327 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsImageEvent.py
+-rw-r--r--   0        0        0     1327 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsVCardEvent.py
+-rw-r--r--   0        0        0     1327 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsVideoEvent.py
+-rw-r--r--   0        0        0      417 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/ISMSEvent.py
+-rw-r--r--   0        0        0      209 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/ISMSMetadata.py
+-rw-r--r--   0        0        0      200 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/ISMSUsage.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/__init__.py
+-rw-r--r--   0        0        0     1385 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/smsEvent.py
+-rw-r--r--   0        0        0     1168 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/smsMetadata.py
+-rw-r--r--   0        0        0     1150 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/smsUsage.py
+-rw-r--r--   0        0        0     1134 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/urlPayload.py
+-rw-r--r--   0        0        0      270 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/viber/IViberEvent.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/viber/__init__.py
+-rw-r--r--   0        0        0     1248 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/viber/viberEvent.py
+-rw-r--r--   0        0        0      328 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/webhookEventTypes.py
+-rw-r--r--   0        0        0      222 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IMessageEventContext.py
+-rw-r--r--   0        0        0      185 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IProfileName.py
+-rw-r--r--   0        0        0      217 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IReplyObject.py
+-rw-r--r--   0        0        0      347 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IWhatsappAudioEvent.py
+-rw-r--r--   0        0        0      501 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IWhatsappEvent.py
+-rw-r--r--   0        0        0      345 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IWhatsappFileEvent.py
+-rw-r--r--   0        0        0      347 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IWhatsappImageEvent.py
+-rw-r--r--   0        0        0      359 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IWhatsappReplyEvent.py
+-rw-r--r--   0        0        0      277 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IWhatsappTextEvent.py
+-rw-r--r--   0        0        0      280 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IWhatsappUnsupportedEvent.py
+-rw-r--r--   0        0        0      347 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/IWhatsappVideoEvent.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/__init__.py
+-rw-r--r--   0        0        0     1210 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/messageEventContext.py
+-rw-r--r--   0        0        0     1148 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/profileName.py
+-rw-r--r--   0        0        0     1189 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/replyObject.py
+-rw-r--r--   0        0        0     1617 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappAudioEvent.py
+-rw-r--r--   0        0        0     1612 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappFileEvent.py
+-rw-r--r--   0        0        0     1617 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappImageEvent.py
+-rw-r--r--   0        0        0     1629 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappReplyEvent.py
+-rw-r--r--   0        0        0     1544 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappTextEvent.py
+-rw-r--r--   0        0        0     1558 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappUnsupportedEvent.py
+-rw-r--r--   0        0        0     1617 2023-05-30 13:25:38.331589 nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappVideoEvent.py
+-rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 nerualpha-5.0.0/PKG-INFO
```

### Comparing `nerualpha-4.1.0rc5/README.md` & `nerualpha-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/pyproject.toml` & `nerualpha-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nerualpha"
-version = "4.1.0rc5"
+version = "5.0.0"
 description = "neru-sdk for python developers"
 authors = ["Sergei Rastrigin <sergei.rastrigin@vonage.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10.5"
@@ -17,15 +17,15 @@
 bumpver = "^2022.1118"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "4.1.0rc5"
+current_version = "5.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/IBridge.py` & `nerualpha-5.0.0/src/nerualpha/IBridge.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.request.IRequestParams import IRequestParams
 from nerualpha.services.config.pathObject import PathObject
-
+T = TypeVar('T')
+K = TypeVar('K')
 
 #interface
 class IBridge(ABC):
     @abstractmethod
-    def encodeUriComponent(self,s):
+    def encodeUriComponent(self,s: str):
         pass
     @abstractmethod
-    def parsePath(self,path):
+    def parsePath(self,path: str):
         pass
     @abstractmethod
-    def testRegEx(self,str,regExp):
+    def testRegEx(self,str: str,regExp: str):
         pass
     @abstractmethod
-    def isInteger(self,value):
+    def isInteger(self,value: int):
         pass
     @abstractmethod
-    def substring(self,str,start,end = None):
+    def substring(self,str: str,start: int,end: int = None):
         pass
     @abstractmethod
-    def jsonStringify(self,data):
+    def jsonStringify(self,data: object):
         pass
     @abstractmethod
-    def jsonParse(self,json):
+    def jsonParse(self,json: str):
         pass
     @abstractmethod
-    def getEnv(self,name):
+    def getEnv(self,name: str):
         pass
     @abstractmethod
-    def request(self,params):
+    def request(self,params: IRequestParams[T]):
         pass
     @abstractmethod
-    def requestWithoutResponse(self,params):
+    def requestWithoutResponse(self,params: IRequestParams[T]):
         pass
     @abstractmethod
     def uuid(self):
         pass
     @abstractmethod
     def isoDate(self):
         pass
     @abstractmethod
-    def runBackgroundTask(self,task):
+    def runBackgroundTask(self,task: object):
         pass
     @abstractmethod
-    def createReadStream(self,path):
+    def createReadStream(self,path: str):
         pass
     @abstractmethod
-    def toISOString(self,seconds):
+    def toISOString(self,seconds: int):
         pass
     @abstractmethod
-    def jwtSign(self,payload,privateKey,alg,options = None):
+    def jwtSign(self,payload: object,privateKey: str,alg: str,options: object = None):
         pass
     @abstractmethod
-    def jwtVerify(self,token,privateKey,algorithm):
+    def jwtVerify(self,token: str,privateKey: str,algorithm: str):
         pass
     @abstractmethod
-    def jwtDecode(self,token):
+    def jwtDecode(self,token: str):
         pass
     @abstractmethod
     def getSystemTime(self):
         pass
     @abstractmethod
-    def log(self,data):
+    def log(self,data: object):
         pass
     @abstractmethod
-    def getObjectKeys(self,obj):
+    def getObjectKeys(self,obj: T):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/INeru.py` & `nerualpha-5.0.0/src/nerualpha/INeru.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from nerualpha.request.IRequest import IRequest
 from nerualpha.session.neruSession import NeruSession
 
 
 #interface
 class INeru(ABC):
     @abstractmethod
-    def createSession(self,ttl = None):
+    def createSession(self,ttl: int = None):
         pass
     @abstractmethod
-    def createSessionWithId(self,id):
+    def createSessionWithId(self,id: str):
         pass
     @abstractmethod
-    def getSessionById(self,id):
+    def getSessionById(self,id: str):
         pass
     @abstractmethod
     def getAppUrl(self):
         pass
     @abstractmethod
-    def getSessionFromRequest(self,req):
+    def getSessionFromRequest(self,req: IRequest):
         pass
     @abstractmethod
     def getGlobalSession(self):
         pass
     @abstractmethod
     def getInstanceState(self):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/bridge.py` & `nerualpha-5.0.0/src/nerualpha/bridge.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/neru.py` & `nerualpha-5.0.0/src/nerualpha/neru.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,45 +24,45 @@
     bridge: IBridge
     def __init__(self):
         self.bridge = Bridge()
         self.config = Config(self.bridge)
         self.jwt = JWT(self.bridge,self.config)
         self.commandService = CommandService(self.bridge)
     
-    def createVonageToken(self,params):
+    def createVonageToken(self,params: ICreateVonageTokenParams):
         if params is None:
             raise Exception("params is required")
         
         if params.exp is None:
             raise Exception("params.exp is required")
         
         return self.jwt.createVonageToken(params)
     
-    def createSession(self,ttl = 7 * 24 * 60 * 60):
+    def createSession(self,ttl: int = 7 * 24 * 60 * 60):
         if self.bridge.isInteger(ttl) is False or ttl < 0:
             raise Exception("ttl must be a positive integer")
         
         id = self.bridge.uuid()
         session = self.createSessionWithId(id)
         self.bridge.runBackgroundTask(session.emitSessionCreatedEvent(ttl))
         return session
     
-    def createSessionWithId(self,id):
+    def createSessionWithId(self,id: str):
         return NeruSession(self.commandService,self.bridge,self.config,self.jwt,id)
     
-    def getSessionById(self,id):
+    def getSessionById(self,id: str):
         if id is None:
             raise Exception("id is required")
         
         return self.createSessionWithId(id)
     
     def getAppUrl(self):
         return self.config.appUrl
     
-    def getSessionFromRequest(self,req):
+    def getSessionFromRequest(self,req: IRequest):
         if req is None:
             raise Exception("getSessionFromRequest: function requires request object to be provided")
         
         if req.headers is None:
             raise Exception("getSessionFromRequest: invalid request object proivided")
         
         id = req.headers["x-neru-sessionid"]
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/IAssets.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/IAssets.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 from nerualpha.providers.assets.contracts.assetLinkResponse import AssetLinkResponse
 from nerualpha.providers.assets.contracts.assetListResponse import AssetListResponse
 
 
 #interface
 class IAssets(ABC):
     @abstractmethod
-    def createDir(self,name):
+    def createDir(self,name: str):
         pass
     @abstractmethod
-    def remove(self,remoteFilePath,recursive):
+    def remove(self,remoteFilePath: str,recursive: bool):
         pass
     @abstractmethod
-    def getRemoteFile(self,remoteFilePath):
+    def getRemoteFile(self,remoteFilePath: str):
         pass
     @abstractmethod
-    def generateLink(self,remoteFilePath,duration):
+    def generateLink(self,remoteFilePath: str,duration: str):
         pass
     @abstractmethod
-    def uploadFiles(self,localFilePaths,remoteDir,retentionPeriod = None):
+    def uploadFiles(self,localFilePaths: List[str],remoteDir: str,retentionPeriod: str = None):
         pass
     @abstractmethod
-    def uploadData(self,data,remoteDir,filenames = None,retentionPeriod = None):
+    def uploadData(self,data: List[object],remoteDir: str,filenames: List[str] = None,retentionPeriod: str = None):
         pass
     @abstractmethod
-    def list(self,remotePath,recursive,limit):
+    def list(self,remotePath: str,recursive: bool,limit: int):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/assets.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,59 +23,59 @@
 
 @dataclass
 class Assets(IAssets):
     bridge: IBridge
     session: ISession
     config: IConfig
     provider: str = field(default = "vonage-assets")
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.session = session
         self.bridge = session.bridge
         self.config = session.config
     
-    def createDir(self,name):
+    def createDir(self,name: str):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = DirectoryPayload(name)
         requestParams.url = self.config.getExecutionUrl(self.provider,AssetsActions.Mkdir)
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def remove(self,remoteFilePath,recursive = False):
+    def remove(self,remoteFilePath: str,recursive: bool = False):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = RemoveAssetPayload(remoteFilePath,recursive)
         requestParams.url = self.config.getExecutionUrl(self.provider,AssetsActions.Remove)
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def getRemoteFile(self,remoteFilePath):
+    def getRemoteFile(self,remoteFilePath: str):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.GET
         requestParams.url = self.config.getExecutionUrl(self.provider,AssetsActions.Binary,{"key": remoteFilePath})
         requestParams.headers = self.session.constructRequestHeaders()
         requestParams.responseType = ResponseTypes.STREAM
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def generateLink(self,remoteFilePath,duration = "5m"):
+    def generateLink(self,remoteFilePath: str,duration: str = "5m"):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = LinkPayload(remoteFilePath,duration)
         requestParams.url = self.config.getExecutionUrl(self.provider,AssetsActions.Link)
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def uploadFiles(self,localFilePaths,remoteDir,retentionPeriod = None):
+    def uploadFiles(self,localFilePaths: List[str],remoteDir: str,retentionPeriod: FileRetentionPeriod = None):
         streams = []
         for i in range(0,localFilePaths.__len__()):
             streams.append(self.bridge.createReadStream(localFilePaths[i]))
         
         return self.uploadData(streams,remoteDir,None,retentionPeriod)
     
-    def uploadData(self,data,remoteDir,filenames = None,retentionPeriod = None):
+    def uploadData(self,data: List[object],remoteDir: str,filenames: List[str] = None,retentionPeriod: FileRetentionPeriod = None):
         url = self.config.getExecutionUrl(self.provider,AssetsActions.Copy,{"dst": remoteDir,"retention": retentionPeriod})
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = []
         for i in range(0,data.__len__()):
             formData = FormDataObject()
             formData.name = f'file[{i}]'
@@ -86,15 +86,15 @@
             requestParams.data.append(formData)
         
         requestParams.url = url
         requestParams.headers = self.session.constructRequestHeaders()
         requestParams.headers["Content-Type"] = "multipart/form-data"
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def list(self,remotePath,recursive = False,limit = 1000):
+    def list(self,remotePath: str,recursive: bool = False,limit: int = 1000):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = ListAssetsPayload(remotePath,recursive,limit)
         requestParams.url = self.config.getExecutionUrl(self.provider,AssetsActions.List)
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetInfo.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/assetInfo.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetLinkResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/assetLinkResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/assetListResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/assetListResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/directoryPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/directoryPayload.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 
 @dataclass
 class DirectoryPayload:
     directory: str
-    def __init__(self,name):
+    def __init__(self,name: str):
         self.directory = name
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/getAssetPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/getAssetPayload.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 
 @dataclass
 class GetAssetPayload:
     key: str
-    def __init__(self,path):
+    def __init__(self,path: str):
         self.key = path
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/getAssetResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/getAssetResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/linkPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/removeAssetPayload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 
 @dataclass
-class LinkPayload:
-    duration: str
-    path: str
-    def __init__(self,path,duration):
-        self.path = path
-        self.duration = duration
+class RemoveAssetPayload:
+    recursive: bool
+    prefix: str
+    def __init__(self,prefix: str,recursive: bool):
+        self.prefix = prefix
+        self.recursive = recursive
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/listAssetsPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/listAssetsPayload.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 @dataclass
 class ListAssetsPayload:
     recursive: bool
     limit: int
     prefix: str
-    def __init__(self,prefix,recursive,limit):
+    def __init__(self,prefix: str,recursive: bool,limit: int):
         self.prefix = prefix
         self.limit = limit
         self.recursive = recursive
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/assets/contracts/removeAssetPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/queueRate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
+from nerualpha.providers.queue.contracts.IQueueRate import IQueueRate
 
 @dataclass
-class RemoveAssetPayload:
-    recursive: bool
-    prefix: str
-    def __init__(self,prefix,recursive):
-        self.prefix = prefix
-        self.recursive = recursive
-    
+class QueueRate(IQueueRate):
+    msgPerSecond: int
+    maxInflight: int
+    def __init__(self):
+        pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/events/eventEmitter.py` & `nerualpha-5.0.0/src/nerualpha/providers/events/eventEmitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 from nerualpha.providers.events.eventFactory import EventFactory
 from nerualpha.providers.events.IEventEmitter import IEventEmitter
 from nerualpha.providers.events.IEventFactory import IEventFactory
 from nerualpha.providers.events.ISessionCreatedDetails import ISessionCreatedDetails
 from nerualpha.providers.events.sessionCreatedDetails import SessionCreatedDetails
 from nerualpha.providers.events.neruEventTypes import NeruEventTypes
 from nerualpha.providers.events.INeruEvent import INeruEvent
-
+T = TypeVar('T')
 @dataclass
 class EventEmitter(IEventEmitter):
     url: str
     session: ISession
     eventFactory: IEventFactory
     bridge: IBridge
     config: IConfig
     provider: str = field(default = "events-submission")
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.config = session.config
         self.bridge = session.bridge
         self.session = session
         self.eventFactory = EventFactory(self.session)
         self.url = self.config.getExecutionUrl(self.provider)
     
-    async def emitSessionCreatedEvent(self,ttl):
+    async def emitSessionCreatedEvent(self,ttl: int):
         expiresAt = self.bridge.toISOString(ttl)
         details = SessionCreatedDetails(expiresAt)
         event = self.eventFactory.createEvent(NeruEventTypes.SESSION_CREATED,details)
         await self.emit(event)
     
-    async def emit(self,e):
+    async def emit(self,e: T):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.url = self.url
         requestParams.data = e
         requestParams.headers = self.session.constructRequestHeaders()
         await self.bridge.requestWithoutResponse(requestParams)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/events/eventFactory.py` & `nerualpha-5.0.0/src/nerualpha/providers/events/eventFactory.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 
 from nerualpha.session.ISession import ISession
 from nerualpha.providers.events.IEventFactory import IEventFactory
 from nerualpha.providers.events.INeruEvent import INeruEvent
 from nerualpha.providers.events.neruEvent import NeruEvent
 from nerualpha.providers.events.neruEventSourceTypes import NeruEventSourceTypes
 from nerualpha.providers.events.neruEventTypes import NeruEventTypes
-
+T = TypeVar('T')
 @dataclass
 class EventFactory(IEventFactory):
     session: ISession
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.session = session
     
-    def createEvent(self,eventName,details):
+    def createEvent(self,eventName: str,details: T):
         if eventName is NeruEventTypes.SESSION_CREATED:
             event = NeruEvent()
             event.event_type = NeruEventTypes.SESSION_CREATED
             event.source_type = NeruEventSourceTypes.INSTANCE
             event.details = details
             self.setCommonFields(event)
             return event
         
         raise Exception("Event type not supported: " + eventName)
     
-    def setCommonFields(self,event):
+    def setCommonFields(self,event: INeruEvent[T]):
         event.timestamp = self.session.bridge.isoDate()
         event.id = self.session.bridge.uuid()
         event.source_id = self.session.config.instanceServiceName
         event.api_account_id = self.session.config.apiAccountId
         event.api_application_id = self.session.config.apiApplicationId
         event.session_id = self.session.id
         event.instance_id = self.session.config.instanceId
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/events/neruEvent.py` & `nerualpha-5.0.0/src/nerualpha/providers/events/neruEvent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.events.INeruEvent import INeruEvent
-
+T = TypeVar('T')
 T = TypeVar("T")
 
 @dataclass
 class NeruEvent(INeruEvent,Generic[T]):
     details: T
     instance_id: str
     session_id: str
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/events/sessionCreatedDetails.py` & `nerualpha-5.0.0/src/nerualpha/providers/events/sessionCreatedDetails.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.events.ISessionCreatedDetails import ISessionCreatedDetails
 
 @dataclass
 class SessionCreatedDetails(ISessionCreatedDetails):
     expiresAt: str
-    def __init__(self,expiresAt):
+    def __init__(self,expiresAt: str):
         self.expiresAt = expiresAt
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logAction.py` & `nerualpha-5.0.0/src/nerualpha/providers/logger/logAction.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logContext.py` & `nerualpha-5.0.0/src/nerualpha/providers/logger/logContext.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nerualpha.providers.logger.ILogContext import ILogContext
 
 @dataclass
 class LogContext(ILogContext):
     result: str
     payload: str
     actionName: str
-    def __init__(self,actionName,payload,result):
+    def __init__(self,actionName: str,payload: str,result: str):
         self.actionName = actionName
         self.payload = payload
         self.result = result
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/logger/logger.py` & `nerualpha-5.0.0/src/nerualpha/providers/logger/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 @dataclass
 class Logger(ILogger):
     url: str
     session: ISession
     bridge: IBridge
     config: IConfig
     provider: str = field(default = "logs-submission")
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.config = session.config
         self.bridge = session.bridge
         self.session = session
         self.url = self.config.getExecutionUrl(self.provider)
     
-    def createLogAction(self,level,message,context = None):
+    def createLogAction(self,level: str,message: str,context: ILogContext = None):
         logAction = LogAction()
         logAction.id = self.bridge.uuid()
         logAction.api_application_id = self.config.apiApplicationId
         logAction.api_account_id = self.config.apiAccountId
         logAction.session_id = self.session.id
         logAction.timestamp = self.bridge.isoDate()
         logAction.log_level = level
@@ -38,15 +38,15 @@
         logAction.source_id = self.config.instanceServiceName
         logAction.instance_id = self.config.instanceId
         if context is not None:
             logAction.context = context
         
         return logAction
     
-    async def log(self,level,message,context = None):
+    async def log(self,level: str,message: str,context: ILogContext = None):
         logAction = self.createLogAction(level,message,context)
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.url = self.url
         requestParams.data = logAction
         requestParams.headers = self.session.constructRequestHeaders()
         await self.bridge.requestWithoutResponse(requestParams)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/createRoomPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/createRoomPayload.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class CreateRoomPayload(ICreateRoomPayload):
     display_name: str
     metadata: str = None
     type_: str = None
     expires_at: str = None
     expire_after_use: bool = None
     recording_options: str = None
-    def __init__(self,display_name,metadata = None,type_ = None,expires_at = None,expire_after_use = None,recording_options = None):
+    def __init__(self,display_name: str,metadata: str = None,type_: str = None,expires_at: str = None,expire_after_use: bool = None,recording_options: str = None):
         self.display_name = display_name
         self.metadata = metadata
         self.type_ = type_
         self.expires_at = expires_at
         self.expire_after_use = expire_after_use
         self.recording_options = recording_options
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/deleteRoomPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/deleteRoomPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/getRoomsResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/getRoomsResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/pageLinks.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/pageLinks.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/recordingOptions.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/recordingOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomLinks.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/roomLinks.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/roomResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/roomsEmbedded.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/roomsEmbedded.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/updateRoomDetails.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/replyObject.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
+from nerualpha.webhookEvents.whatsapp.IReplyObject import IReplyObject
 
 @dataclass
-class UpdateRoomDetails:
-    expire_after_use: bool
-    expires_at: str
-    def __init__(self,expires_at,expire_after_use):
-        self.expires_at = expires_at
-        self.expire_after_use = expire_after_use
-    
+class ReplyObject(IReplyObject):
+    title: str
+    id: str
+    description: str = None
+    def __init__(self):
+        pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/contracts/updateRoomPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/updateRoomPayload.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.meetings.contracts.updateRoomDetails import UpdateRoomDetails
 
 @dataclass
 class UpdateRoomPayload:
     update_details: UpdateRoomDetails
-    def __init__(self,update_details):
+    def __init__(self,update_details: UpdateRoomDetails):
         self.update_details = update_details
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/meetings/meetings.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/meetings.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,45 +16,45 @@
 from nerualpha.request.requestMethods import RequestMethods
 
 @dataclass
 class Meetings:
     baseUrl: str
     vonageAPI: IVonageAPI
     session: ISession
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.session = session
         self.vonageAPI = VonageAPI(self.session)
         self.baseUrl = "https://api-eu.vonage.com/beta/meetings"
     
-    def getRoom(self,roomId):
+    def getRoom(self,roomId: str):
         url = f'{self.baseUrl}/rooms/{roomId}'
         method = RequestMethods.GET
         return self.vonageAPI.invoke(url,method,None)
     
-    def getRooms(self,paginationUrl = None):
+    def getRooms(self,paginationUrl: str = None):
         url = f'{self.baseUrl}/rooms'
         if paginationUrl is not None:
             url = paginationUrl
         
         method = RequestMethods.GET
         return self.vonageAPI.invoke(url,method,None)
     
-    def createRoom(self,createRoomPayload):
+    def createRoom(self,createRoomPayload: ICreateRoomPayload):
         url = f'{self.baseUrl}/rooms'
         method = RequestMethods.POST
         return self.vonageAPI.invoke(url,method,createRoomPayload)
     
-    def updateRoom(self,roomId,expiry,expireAfterUse):
+    def updateRoom(self,roomId: str,expiry: str,expireAfterUse: bool):
         details = UpdateRoomDetails(expiry,expireAfterUse)
         payload = UpdateRoomPayload(details)
         url = f'{self.baseUrl}/rooms/{roomId}'
         method = RequestMethods.PATCH
         return self.vonageAPI.invoke(url,method,payload)
     
-    def deleteRoom(self,roomId):
+    def deleteRoom(self,roomId: str):
         url = f'{self.baseUrl}/rooms/{roomId}'
         method = RequestMethods.DEL
         payload = DeleteRoomPayload()
         return self.vonageAPI.invoke(url,method,payload)
     
     def reprJSON(self):
         result = {}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/IMessages.py` & `nerualpha-5.0.0/src/nerualpha/providers/queue/IQueue.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.session.requestInterface import RequestInterface
-from nerualpha.session.requestInterfaceForCallbacks import RequestInterfaceForCallbacks
-from nerualpha.providers.vonageAPI.contracts.invokePayload import InvokePayload
-from nerualpha.providers.messages.contracts.IBaseMessage import IBaseMessage
-from nerualpha.providers.messages.contracts.IMessageContact import IMessageContact
-from nerualpha.providers.messages.contracts.ISendImageContent import ISendImageContent
-from nerualpha.providers.messages.contracts.sendImagePayload import SendImagePayload
-from nerualpha.providers.messages.contracts.sendTextPayload import SendTextPayload
-from nerualpha.providers.messages.contracts.unsubscribeEventsPayload import UnsubscribeEventsPayload
-from nerualpha.providers.messages.contracts.sendResponse import SendResponse
-
+from nerualpha.IBridge import IBridge
+from nerualpha.services.config.IConfig import IConfig
+from nerualpha.session.ISession import ISession
+from nerualpha.providers.queue.contracts.ICreateQueueOptions import ICreateQueueOptions
+from nerualpha.session.requestInterfaceWithParams import RequestInterfaceWithParams
+from nerualpha.providers.queue.contracts.ICreateQueuePayload import ICreateQueuePayload
+from nerualpha.providers.queue.contracts.queueDetailsResponse import QueueDetailsResponse
+from nerualpha.providers.queue.contracts.IUpdateQueueOptions import IUpdateQueueOptions
+from nerualpha.providers.queue.contracts.IUpdateQueuePayload import IUpdateQueuePayload
+T = TypeVar('T')
 
 #interface
-class IMessages(ABC):
+class IQueue(ABC):
+    config:IConfig
+    provider:str
+    session:ISession
+    bridge:IBridge
+    @abstractmethod
+    def createQueue(self,queueName: str,callback: str,options: ICreateQueueOptions):
+        pass
+    @abstractmethod
+    def updateQueue(self,queueName: str,options: IUpdateQueueOptions):
+        pass
+    @abstractmethod
+    def list(self):
+        pass
     @abstractmethod
-    def send(self,message):
+    def getQueueDetails(self,name: str):
         pass
     @abstractmethod
-    def sendText(self,from_,to,message):
+    def deleteQueue(self,name: str):
         pass
     @abstractmethod
-    def sendImage(self,from_,to,imageContent):
+    def pauseQueue(self,name: str):
         pass
     @abstractmethod
-    def listenMessages(self,from_,to,callback):
+    def resumeQueue(self,name: str):
         pass
     @abstractmethod
-    def listenEvents(self,from_,to,callback):
+    def enqueue(self,name: str,data: List[T]):
         pass
     @abstractmethod
-    def onMessage(self,callback,from_,to):
+    def enqueueSingle(self,name: str,data: T):
         pass
     @abstractmethod
-    def onMessageEvents(self,callback,from_,to):
+    def deadLetterList(self,name: str):
         pass
     @abstractmethod
-    def unsubscribeEvents(self,id):
+    def deadLetterDequeue(self,name: str,count: int):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/baseMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/baseMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/imageData.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/imageData.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from nerualpha.providers.messages.contracts.IImageData import IImageData
 
 @dataclass
 class ImageData(IImageData):
     caption: str
     url: str
-    def __init__(self,url,caption):
+    def __init__(self,url: str,caption: str):
         self.url = url
         self.caption = caption
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/listenEventsPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/listenEventsPayload.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from nerualpha.session.IWrappedCallback import IWrappedCallback
 
 @dataclass
 class ListenEventsPayload(IListenEventsPayload):
     callback: IWrappedCallback
     to: IMessageContact
     from_: IMessageContact
-    def __init__(self,from_,to,callback):
+    def __init__(self,from_: IMessageContact,to: IMessageContact,callback: IWrappedCallback):
         self.from_ = from_
         self.to = to
         self.callback = callback
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/listenMessagesPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/listenMessagesPayload.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from nerualpha.session.IWrappedCallback import IWrappedCallback
 
 @dataclass
 class ListenMessagesPayload(IListenMessagesPayload):
     callback: IWrappedCallback
     to: IMessageContact
     from_: IMessageContact
-    def __init__(self,from_,to,callback):
+    def __init__(self,from_: IMessageContact,to: IMessageContact,callback: IWrappedCallback):
         self.from_ = from_
         self.to = to
         self.callback = callback
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messageContact.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messageContact.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerAudioMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerAudioMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerFileMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerFileMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerImageMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerImageMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerTextMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerTextMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/messengerVideoMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/messengerVideoMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsAudioMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/mmsAudioMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsImageMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/mmsImageMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsVCardMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/mmsVCardMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/mmsVideoMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/mmsVideoMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImageContent.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendImageContent.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nerualpha.providers.messages.contracts.IImageData import IImageData
 from nerualpha.providers.messages.contracts.ISendImageContent import ISendImageContent
 
 @dataclass
 class SendImageContent(ISendImageContent):
     image: IImageData
     type_: str = field(default = "image")
-    def __init__(self,imageData):
+    def __init__(self,imageData: IImageData):
         self.image = imageData
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImageMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendImageMessage.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from nerualpha.providers.messages.contracts.ISendImageContent import ISendImageContent
 from nerualpha.providers.messages.contracts.ISendImageMessage import ISendImageMessage
 
 @dataclass
 class SendImageMessage(ISendImageMessage):
     content: ISendImageContent
-    def __init__(self,content):
+    def __init__(self,content: ISendImageContent):
         self.content = content
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendImagePayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendImagePayload.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from nerualpha.providers.messages.contracts.sendImageMessage import SendImageMessage
 
 @dataclass
 class SendImagePayload(ISendImagePayload):
     message: SendImageMessage
     to: IMessageContact
     from_: IMessageContact
-    def __init__(self,from_,to,message):
+    def __init__(self,from_: IMessageContact,to: IMessageContact,message: SendImageContent):
         self.from_ = from_
         self.to = to
         if message.type_ is None:
             message.type_ = "image"
         
         self.message = SendImageMessage(message)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextContent.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendTextContent.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from nerualpha.providers.messages.contracts.ISendTextContent import ISendTextContent
 
 @dataclass
 class SendTextContent(ISendTextContent):
     text: str
     type_: str
-    def __init__(self,text):
+    def __init__(self,text: str):
         self.type_ = "text"
         self.text = text
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextMessagePayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendTextMessagePayload.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from nerualpha.providers.messages.contracts.ISendTextMessagePayload import ISendTextMessagePayload
 from nerualpha.providers.messages.contracts.ISendTextContent import ISendTextContent
 
 @dataclass
 class SendTextMessagePayload(ISendTextMessagePayload):
     content: ISendTextContent
-    def __init__(self,content):
+    def __init__(self,content: ISendTextContent):
         self.content = content
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/sendTextPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/sendTextPayload.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from nerualpha.providers.messages.contracts.sendTextContent import SendTextContent
 
 @dataclass
 class SendTextPayload(ISendTextPayload):
     message: ISendTextMessagePayload
     to: IMessageContact
     from_: IMessageContact
-    def __init__(self,from_,to,text):
+    def __init__(self,from_: IMessageContact,to: IMessageContact,text: str):
         self.from_ = from_
         self.to = to
         self.message = SendTextMessagePayload(SendTextContent(text))
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/smsMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/smsMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/unsubscribeEventsPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/unsubscribeEventsPayload.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.messages.contracts.IUnsubscribeEventsPayload import IUnsubscribeEventsPayload
 
 @dataclass
 class UnsubscribeEventsPayload(IUnsubscribeEventsPayload):
     id: str
-    def __init__(self,id):
+    def __init__(self,id: str):
         self.id = id
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/urlPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/urlPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/viberImageMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/viberImageMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/viberTextMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/viberTextMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappAudioMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappAudioMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappFileMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappFileMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappImageMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappImageMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappTemplateMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappTemplateMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappTextMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappTextMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/contracts/whatsappVideoMessage.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/contracts/whatsappVideoMessage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/messages/messages.py` & `nerualpha-5.0.0/src/nerualpha/providers/messages/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,58 +22,61 @@
 from nerualpha.providers.vonageAPI.contracts.invokePayload import InvokePayload
 from nerualpha.providers.messages.contracts.sendResponse import SendResponse
 
 @dataclass
 class Messages(IMessages):
     vonageAPI: IVonageAPI
     session: ISession
-    baseUrl: str = field(default = "https://api.nexmo.com")
+    regionURL: str = field(default = "https://api.nexmo.com")
     provider: str = field(default = "vonage-messaging")
-    def __init__(self,session):
+    def __init__(self,session: ISession,regionURL: str = None):
         self.session = session
         self.vonageAPI = VonageAPI(self.session)
+        if regionURL is not None:
+            self.regionURL = regionURL
+        
     
-    def send(self,message):
-        url = f'{self.baseUrl}/v1/messages'
+    def send(self,message: IBaseMessage):
+        url = f'{self.regionURL}/v1/messages'
         method = "POST"
         return self.vonageAPI.invoke(url,method,message)
     
-    def sendText(self,from_,to,message):
+    def sendText(self,from_: IMessageContact,to: IMessageContact,message: str):
         payload = SendTextPayload(from_,to,message)
-        url = f'{self.baseUrl}/v0.1/messages'
+        url = f'{self.regionURL}/v0.1/messages'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def sendImage(self,from_,to,imageContent):
+    def sendImage(self,from_: IMessageContact,to: IMessageContact,imageContent: ISendImageContent):
         payload = SendImagePayload(from_,to,imageContent)
-        url = f'{self.baseUrl}/v0.1/messages'
+        url = f'{self.regionURL}/v0.1/messages'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def listenMessages(self,from_,to,callback):
+    def listenMessages(self,from_: IMessageContact,to: IMessageContact,callback: str):
         payload = ListenMessagesPayload(from_,to,self.session.wrapCallback(callback,[]))
         action = ActionPayload(self.provider,MessageActions.SubscribeInboundMessages,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    def listenEvents(self,from_,to,callback):
+    def listenEvents(self,from_: IMessageContact,to: IMessageContact,callback: str):
         payload = ListenEventsPayload(from_,to,self.session.wrapCallback(callback,[]))
         action = ActionPayload(self.provider,MessageActions.SubscribeInboundEvents,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    def onMessage(self,callback,from_,to):
+    def onMessage(self,callback: str,from_: IMessageContact,to: IMessageContact):
         payload = ListenMessagesPayload(from_,to,self.session.wrapCallback(callback,[]))
         action = ActionPayload(self.provider,MessageActions.SubscribeInboundMessages,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    def onMessageEvents(self,callback,from_,to):
+    def onMessageEvents(self,callback: str,from_: IMessageContact,to: IMessageContact):
         payload = ListenEventsPayload(from_,to,self.session.wrapCallback(callback,[]))
         action = ActionPayload(self.provider,MessageActions.SubscribeInboundEvents,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    def unsubscribeEvents(self,id):
+    def unsubscribeEvents(self,id: str):
         payload = UnsubscribeEventsPayload(id)
         action = ActionPayload(self.provider,MessageActions.UnsubscribeEvents,payload)
         return RequestInterface(self.session,action)
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/baseNumberOptions.py` & `nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/baseNumberOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/getNumbersOptions.py` & `nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/getNumbersOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/getNumbersResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/getNumbersResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numberOptions.py` & `nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/numberOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numberResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/numberResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/numbersOperationResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/numbersOperationResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/searchNumbersOptions.py` & `nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/searchNumbersOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/contracts/updateNumberOptions.py` & `nerualpha-5.0.0/src/nerualpha/providers/numbers/contracts/updateNumberOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/numbers/numbers.py` & `nerualpha-5.0.0/src/nerualpha/providers/numbers/numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 @dataclass
 class Numbers:
     bridge: IBridge
     accountUrl: str
     baseUrl: str
     vonageAPI: IVonageAPI
     session: ISession
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.session = session
         self.bridge = session.bridge
         self.vonageAPI = VonageAPI(self.session)
         self.baseUrl = "https://rest.nexmo.com/number"
         self.accountUrl = "https://rest.nexmo.com/account/numbers"
     
-    def getNumbers(self,apiKey,apiSecret,getNumberOptions = None):
+    def getNumbers(self,apiKey: str,apiSecret: str,getNumberOptions: IGetNumbersOptions = None):
         url = f'{self.accountUrl}?api_key={apiKey}&api_secret={apiSecret}'
         options = {}
         if getNumberOptions.application_id is not None:
             options["application_id"] = getNumberOptions.application_id
         
         if getNumberOptions.has_application is not None:
             options["has_application"] = getNumberOptions.has_application
@@ -53,15 +53,15 @@
         if getNumberOptions.index is not None:
             options["index"] = getNumberOptions.index
         
         url = self.buildUrl(url,options)
         method = "GET"
         return self.vonageAPI.invoke(url,method,None)
     
-    def searchNumbers(self,apiKey,apiSecret,searchNumberOptions):
+    def searchNumbers(self,apiKey: str,apiSecret: str,searchNumberOptions: ISearchNumbersOptions):
         url = f'{self.baseUrl}/search?api_key={apiKey}&api_secret={apiSecret}'
         options = {}
         if searchNumberOptions.country is not None:
             options["country"] = searchNumberOptions.country
         
         if searchNumberOptions.type_ is not None:
             options["type_"] = searchNumberOptions.type_
@@ -81,15 +81,15 @@
         if searchNumberOptions.index is not None:
             options["index"] = searchNumberOptions.index
         
         url = self.buildUrl(url,options)
         method = "GET"
         return self.vonageAPI.invoke(url,method,None)
     
-    def buyNumber(self,apiKey,apiSecret,numberOptions):
+    def buyNumber(self,apiKey: str,apiSecret: str,numberOptions: INumberOptions):
         url = f'{self.baseUrl}/buy?api_key={apiKey}&api_secret={apiSecret}'
         options = {}
         if numberOptions.country is not None:
             options["country"] = numberOptions.country
         
         if numberOptions.msisdn is not None:
             options["msisdn"] = numberOptions.msisdn
@@ -97,15 +97,15 @@
         if numberOptions.target_api_key is not None:
             options["target_api_key"] = numberOptions.target_api_key
         
         url = self.buildUrl(url,options)
         method = "POST"
         return self.vonageAPI.invoke(url,method,None)
     
-    def cancelNumber(self,apiKey,apiSecret,numberOptions):
+    def cancelNumber(self,apiKey: str,apiSecret: str,numberOptions: INumberOptions):
         url = f'{self.baseUrl}/cancel?api_key={apiKey}&api_secret={apiSecret}'
         options = {}
         if numberOptions.country is not None:
             options["country"] = numberOptions.country
         
         if numberOptions.msisdn is not None:
             options["msisdn"] = numberOptions.msisdn
@@ -113,15 +113,15 @@
         if numberOptions.target_api_key is not None:
             options["target_api_key"] = numberOptions.target_api_key
         
         url = self.buildUrl(url,options)
         method = "POST"
         return self.vonageAPI.invoke(url,method,None)
     
-    def updateNumber(self,apiKey,apiSecret,updateNumberOptions):
+    def updateNumber(self,apiKey: str,apiSecret: str,updateNumberOptions: IUpdateNumberOptions):
         url = f'{self.baseUrl}/update?api_key={apiKey}&api_secret={apiSecret}'
         options = {}
         if updateNumberOptions.country is not None:
             options["country"] = updateNumberOptions.country
         
         if updateNumberOptions.msisdn is not None:
             options["msisdn"] = updateNumberOptions.msisdn
@@ -144,15 +144,15 @@
         if updateNumberOptions.voiceStatusCallback is not None:
             options["voiceStatusCallback"] = updateNumberOptions.voiceStatusCallback
         
         url = self.buildUrl(url,options)
         method = "POST"
         return self.vonageAPI.invoke(url,method,None)
     
-    def buildUrl(self,baseUrl,options):
+    def buildUrl(self,baseUrl: str,options: Dict[str,object]):
         keys = self.bridge.getObjectKeys(options)
         queryString = ""
         for i in range(0,keys.__len__()):
             key = keys[i]
             value = options[key]
             queryString += f'{key}={value}'
             if i + 1 < keys.__len__():
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/IQueue.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/IUsers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,31 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.IBridge import IBridge
-from nerualpha.services.config.IConfig import IConfig
-from nerualpha.session.ISession import ISession
-from nerualpha.providers.queue.contracts.ICreateQueueOptions import ICreateQueueOptions
-from nerualpha.session.requestInterfaceWithParams import RequestInterfaceWithParams
-from nerualpha.providers.queue.contracts.ICreateQueuePayload import ICreateQueuePayload
-from nerualpha.providers.queue.contracts.queueDetailsResponse import QueueDetailsResponse
-from nerualpha.providers.queue.contracts.IUpdateQueueOptions import IUpdateQueueOptions
-from nerualpha.providers.queue.contracts.IUpdateQueuePayload import IUpdateQueuePayload
+from nerualpha.session.requestInterface import RequestInterface
+from nerualpha.providers.vonageAPI.contracts.invokePayload import InvokePayload
+from nerualpha.providers.voice.contracts.createUserPayload import CreateUserPayload
+from nerualpha.providers.voice.contracts.userResponse import UserResponse
+from nerualpha.providers.voice.contracts.getUsersResponse import GetUsersResponse
+from nerualpha.providers.voice.contracts.updateUserPayload import UpdateUserPayload
+from nerualpha.providers.voice.contracts.ICreateUserPayload import ICreateUserPayload
+from nerualpha.providers.voice.contracts.IUpdateUserPayload import IUpdateUserPayload
 
 
 #interface
-class IQueue(ABC):
-    config:IConfig
-    provider:str
-    session:ISession
-    bridge:IBridge
+class IUsers(ABC):
     @abstractmethod
-    def createQueue(self,queueName,callback,options):
+    def getUsers(self,page_size: int = None,order: str = None,pageUrl: str = None):
         pass
     @abstractmethod
-    def updateQueue(self,queueName,options):
+    def getUser(self,user_id: str = None):
         pass
     @abstractmethod
-    def list(self):
+    def createUser(self,createUserPayload: ICreateUserPayload):
         pass
     @abstractmethod
-    def getQueueDetails(self,name):
+    def updateUser(self,user_id: str,updateUserPayload: IUpdateUserPayload):
         pass
     @abstractmethod
-    def deleteQueue(self,name):
-        pass
-    @abstractmethod
-    def pauseQueue(self,name):
-        pass
-    @abstractmethod
-    def resumeQueue(self,name):
-        pass
-    @abstractmethod
-    def enqueue(self,name,data):
-        pass
-    @abstractmethod
-    def enqueueSingle(self,name,data):
-        pass
-    @abstractmethod
-    def deadLetterList(self,name):
-        pass
-    @abstractmethod
-    def deadLetterDequeue(self,name,count):
+    def deleteUser(self,user_id: str):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/createQueueOptions.py` & `nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/createQueueOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/createQueuePayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/createQueuePayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/queueRate.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/userEmbedded.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.providers.queue.contracts.IQueueRate import IQueueRate
+from nerualpha.providers.voice.contracts.user import User
 
 @dataclass
-class QueueRate(IQueueRate):
-    msgPerSecond: int
-    maxInflight: int
+class UserEmbedded:
+    user: User
     def __init__(self):
         pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/updateQueueOptions.py` & `nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/updateQueueOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/contracts/updateQueuePayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/queue/contracts/updateQueuePayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/queue/queue.py` & `nerualpha-5.0.0/src/nerualpha/providers/queue/queue.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,42 +13,42 @@
 from nerualpha.request.requestParams import RequestParams
 from nerualpha.request.requestMethods import RequestMethods
 from nerualpha.session.requestInterfaceWithParams import RequestInterfaceWithParams
 from nerualpha.providers.queue.contracts.queueDetailsResponse import QueueDetailsResponse
 from nerualpha.providers.queue.contracts.IUpdateQueueOptions import IUpdateQueueOptions
 from nerualpha.providers.queue.contracts.updateQueuePayload import UpdateQueuePayload
 from nerualpha.providers.queue.contracts.IUpdateQueuePayload import IUpdateQueuePayload
-
+T = TypeVar('T')
 @dataclass
 class Queue(IQueue):
     session: ISession
     config: IConfig
     bridge: IBridge
     provider: str = field(default = "queue-service")
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.session = session
         self.bridge = session.bridge
         self.config = session.config
     
-    def createQueue(self,name,callback,options):
+    def createQueue(self,name: str,callback: str,options: ICreateQueueOptions):
         payload = CreateQueuePayload()
         payload.name = name
         payload.callback = self.session.wrapCallback(callback,[])
         payload.active = options.active
         payload.rate = QueueRate()
         payload.rate.maxInflight = options.maxInflight
         payload.rate.msgPerSecond = options.msgPerSecond
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = payload
         requestParams.url = self.config.getExecutionUrl(self.provider,"queue")
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def updateQueue(self,queueName,options):
+    def updateQueue(self,queueName: str,options: IUpdateQueueOptions):
         payload = UpdateQueuePayload()
         payload.rate = QueueRate()
         payload.rate.maxInflight = options.maxInflight
         payload.rate.msgPerSecond = options.msgPerSecond
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = payload
@@ -60,66 +60,66 @@
         requestParams = RequestParams()
         requestParams.method = RequestMethods.GET
         requestParams.data = None
         requestParams.url = self.config.getExecutionUrl(self.provider,"queue")
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def getQueueDetails(self,name):
+    def getQueueDetails(self,name: str):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.GET
         requestParams.data = None
         requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}')
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def deleteQueue(self,name):
+    def deleteQueue(self,name: str):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.DEL
         requestParams.data = None
         requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}')
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def pauseQueue(self,name):
+    def pauseQueue(self,name: str):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.PUT
         requestParams.data = None
         requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}/pause')
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def resumeQueue(self,name):
+    def resumeQueue(self,name: str):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.PUT
         requestParams.data = None
         requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}/resume')
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def enqueue(self,name,data):
+    def enqueue(self,name: str,data: List[T]):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = data
         requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}/enqueue')
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def enqueueSingle(self,name,data):
+    def enqueueSingle(self,name: str,data: T):
         return self.enqueue(name,[data])
     
-    def deadLetterList(self,name):
+    def deadLetterList(self,name: str):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.GET
         requestParams.data = None
         requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}/deadletter')
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
     
-    def deadLetterDequeue(self,name,count = 1):
+    def deadLetterDequeue(self,name: str,count: int = 1):
         requestParams = RequestParams()
         requestParams.method = RequestMethods.POST
         requestParams.data = None
         requestParams.url = self.config.getExecutionUrl(self.provider,f'queue/{name}/deadletter/pop',{"count": self.bridge.jsonStringify(count)})
         requestParams.headers = self.session.constructRequestHeaders()
         return RequestInterfaceWithParams(self.session,requestParams)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/IScheduler.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/IScheduler.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from nerualpha.session.requestInterface import RequestInterface
 from nerualpha.session.requestInterfaceForCallbacks import RequestInterfaceForCallbacks
 from nerualpha.providers.scheduler.contracts.schedulerPayload import SchedulerPayload
 from nerualpha.providers.scheduler.contracts.IStartAtParams import IStartAtParams
 from nerualpha.providers.scheduler.contracts.listAllSchedulersResponse import ListAllSchedulersResponse
 from nerualpha.providers.scheduler.contracts.getSchedulerResponse import GetSchedulerResponse
 from nerualpha.providers.scheduler.contracts.listAllPayload import ListAllPayload
-
+T = TypeVar('T')
 
 #interface
 class IScheduler(ABC):
     @abstractmethod
-    def startAt(self,params):
+    def startAt(self,params: IStartAtParams[T]):
         pass
     @abstractmethod
-    def listAll(self,size = None,cursor = None):
+    def listAll(self,size: int = None,cursor: str = None):
         pass
     @abstractmethod
-    def get(self,scheduleId):
+    def get(self,scheduleId: str):
         pass
     @abstractmethod
-    def cancel(self,scheduleId):
+    def cancel(self,scheduleId: str):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/getSchedulerResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/getSchedulerResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/intervalParams.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/intervalParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/listAllPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/listAllPayload.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from nerualpha.providers.scheduler.contracts.IListAllPayload import IListAllPayload
 
 @dataclass
 class ListAllPayload(IListAllPayload):
     cursor: str
     page_size: int
-    def __init__(self,page_size,cursor):
+    def __init__(self,page_size: int,cursor: str):
         self.page_size = page_size
         if cursor is not None:
             self.cursor = cursor
         
     
     def reprJSON(self):
         result = {}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/listAllSchedulersResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/listAllSchedulersResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/schedulerExecutionInfo.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/schedulerExecutionInfo.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/schedulerPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/Link.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.providers.scheduler.contracts.ISchedulePayload import ISchedulePayload
 
 @dataclass
-class SchedulerPayload(ISchedulePayload):
-    id: str
-    def __init__(self,id):
-        self.id = id
-    
+class Link:
+    href: str = None
+    def __init__(self):
+        pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/startAtParams.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/startAtParams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.scheduler.contracts.IIntervalParams import IIntervalParams
 from nerualpha.providers.scheduler.contracts.IStartAtParams import IStartAtParams
-
+T = TypeVar('T')
 T = TypeVar("T")
 
 @dataclass
 class StartAtParams(IStartAtParams,Generic[T]):
     callback: str
     startAt: str
     id: str = None
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/startAtPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/startAtPayload.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.session.IWrappedCallback import IWrappedCallback
 from nerualpha.providers.scheduler.contracts.IIntervalParams import IIntervalParams
 from nerualpha.providers.scheduler.contracts.IStartAtPayload import IStartAtPayload
-
+T = TypeVar('T')
 T = TypeVar("T")
 
 @dataclass
 class StartAtPayload(IStartAtPayload,Generic[T]):
     callback: IWrappedCallback
     startAt: str
     interval: IIntervalParams = None
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/contracts/untilParams.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/untilParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/scheduler/scheduler.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 from nerualpha.session.requestInterfaceForCallbacks import RequestInterfaceForCallbacks
 from nerualpha.session.IPayloadWithCallback import IPayloadWithCallback
 from nerualpha.providers.scheduler.contracts.listAllSchedulersResponse import ListAllSchedulersResponse
 from nerualpha.providers.scheduler.contracts.getSchedulerResponse import GetSchedulerResponse
 from nerualpha.providers.scheduler.contracts.listAllPayload import ListAllPayload
 from nerualpha.providers.scheduler.contracts.IListAllPayload import IListAllPayload
 from nerualpha.IBridge import IBridge
-
+T = TypeVar('T')
 @dataclass
 class Scheduler(IScheduler):
     bridge: IBridge
     session: ISession
     provider: str = field(default = "vonage-scheduler")
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.session = session
         self.bridge = session.bridge
     
-    def startAt(self,params):
+    def startAt(self,params: IStartAtParams[T]):
         if params.id is not None and self.bridge.testRegEx(params.id,"^[a-zA-Z0-9][a-zA-Z0-9-_]*$") is not True:
             raise Exception("Error: The input does not match the required pattern ^[a-zA-Z0-9][a-zA-Z0-9-_]*$. Please enter a string that starts with a letter or a digit, and contains only letters, digits, hyphens, and underscores.")
         
         startAtPayload = StartAtPayload()
         startAtPayload.startAt = params.startAt
         startAtPayload.callback = self.session.wrapCallback(params.callback,[])
         if params.payload is not None:
@@ -42,25 +42,25 @@
         
         if params.id is not None:
             startAtPayload.id = params.id
         
         action = ActionPayload(self.provider,SchedulerActions.Create,startAtPayload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    def listAll(self,size = 10,cursor = None):
+    def listAll(self,size: int = 10,cursor: str = None):
         payload = ListAllPayload(size,cursor)
         action = ActionPayload(self.provider,SchedulerActions.List,payload)
         return RequestInterface(self.session,action)
     
-    def get(self,scheduleId):
+    def get(self,scheduleId: str):
         payload = SchedulerPayload(scheduleId)
         action = ActionPayload(self.provider,SchedulerActions.Get,payload)
         return RequestInterface(self.session,action)
     
-    def cancel(self,scheduleId):
+    def cancel(self,scheduleId: str):
         payload = SchedulerPayload(scheduleId)
         action = ActionPayload(self.provider,SchedulerActions.Cancel,payload)
         return RequestInterface(self.session,action)
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/state/IState.py` & `nerualpha-5.0.0/src/nerualpha/providers/state/IState.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.state.expireOptions import ExpireOptions
-
+T = TypeVar('T')
 
 #interface
 class IState(ABC):
     @abstractmethod
-    def set(self,key,value):
+    def set(self,key: str,value: T):
         pass
     @abstractmethod
-    def get(self,key):
+    def get(self,key: str):
         pass
     @abstractmethod
-    def delete(self,key):
+    def delete(self,key: str):
         pass
     @abstractmethod
-    def hdel(self,htable,key):
+    def hdel(self,htable: str,keys: List[str]):
         pass
     @abstractmethod
-    def hexists(self,htable,key):
+    def hexists(self,htable: str,key: str):
         pass
     @abstractmethod
-    def hgetall(self,htable):
+    def hgetall(self,htable: str):
         pass
     @abstractmethod
-    def hmget(self,htable,keys):
+    def hmget(self,htable: str,keys: List[str]):
         pass
     @abstractmethod
-    def hvals(self,htable):
+    def hvals(self,htable: str):
         pass
     @abstractmethod
-    def hget(self,htable,key):
+    def hget(self,htable: str,key: str):
         pass
     @abstractmethod
-    def hincrby(self,htable,key,value):
+    def hincrby(self,htable: str,key: str,value: int):
         pass
     @abstractmethod
-    def hlen(self,htable):
+    def hlen(self,htable: str):
         pass
     @abstractmethod
-    def hset(self,htable,keyValuePairs):
+    def hset(self,htable: str,keyValuePairs: Dict[str,str]):
         pass
     @abstractmethod
-    def rpush(self,list,value):
+    def rpush(self,list: str,value: T):
         pass
     @abstractmethod
-    def lpush(self,list,value):
+    def lpush(self,list: str,value: T):
         pass
     @abstractmethod
-    def rpop(self,list,count):
+    def rpop(self,list: str,count: int):
         pass
     @abstractmethod
-    def lpop(self,list,count):
+    def lpop(self,list: str,count: int):
         pass
     @abstractmethod
-    def lrem(self,list,value,count):
+    def lrem(self,list: str,value: T,count: int):
         pass
     @abstractmethod
-    def ltrim(self,list,startPos,endPos):
+    def ltrim(self,list: str,startPos: int,endPos: int):
         pass
     @abstractmethod
-    def linsert(self,list,before,pivot,value):
+    def linsert(self,list: str,before: bool,pivot: T,value: T):
         pass
     @abstractmethod
-    def lindex(self,list,position):
+    def lindex(self,list: str,position: int):
         pass
     @abstractmethod
-    def lset(self,list,position,value):
+    def lset(self,list: str,position: int,value: T):
         pass
     @abstractmethod
-    def incrby(self,key,value):
+    def incrby(self,key: str,value: int):
         pass
     @abstractmethod
-    def decrby(self,key,value):
+    def decrby(self,key: str,value: int):
         pass
     @abstractmethod
-    def expire(self,key,seconds,option = None):
+    def expire(self,key: str,seconds: int,option: ExpireOptions = None):
         pass
     @abstractmethod
-    def llen(self,list):
+    def llen(self,list: str):
         pass
     @abstractmethod
-    def lrange(self,list,startPos,endPos):
+    def lrange(self,list: str,startPos: int,endPos: int):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/state/state.py` & `nerualpha-5.0.0/src/nerualpha/providers/state/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,220 +7,220 @@
 from nerualpha.session.ISession import ISession
 from nerualpha.providers.state.IState import IState
 from nerualpha.providers.state.IStateCommand import IStateCommand
 from nerualpha.providers.state.stateCommand import StateCommand
 from nerualpha.providers.state.stateOperations import StateOperations
 from nerualpha.request.requestMethods import RequestMethods
 from nerualpha.providers.state.expireOptions import ExpireOptions
-
+T = TypeVar('T')
 @dataclass
 class State(IState):
     commandService: ICommandService
     session: ISession
     bridge: IBridge
     url: str
     namespace: str
     provider: str = field(default = "client-persistence-api")
-    def __init__(self,session,namespace = None):
+    def __init__(self,session: ISession,namespace: str = None):
         self.bridge = session.bridge
         self.url = session.config.getExecutionUrl(self.provider)
         if namespace is None:
             self.namespace = f'state:{session.id}'
         
         else: 
             self.namespace = namespace
         
         self.session = session
         self.commandService = session.commandService
     
-    def createCommand(self,op,key,args):
+    def createCommand(self,op: str,key: str,args: List[str]):
         return StateCommand(op,self.namespace,key,args)
     
-    async def executeCommand(self,command):
+    async def executeCommand(self,command: IStateCommand):
         return await self.commandService.executeCommand(self.url,RequestMethods.POST,command,self.session.constructRequestHeaders())
     
-    async def set(self,key,value):
+    async def set(self,key: str,value: T):
         payload = []
         payload.append(self.bridge.jsonStringify(value))
         command = self.createCommand(StateOperations.SET,key,payload)
         return await self.executeCommand(command)
     
-    async def get(self,key):
+    async def get(self,key: str):
         payload = []
         command = self.createCommand(StateOperations.GET,key,payload)
         result = await self.executeCommand(command)
         if result is not None and result != "":
             return self.bridge.jsonParse(result)
         
         return None
     
-    async def delete(self,key):
+    async def delete(self,key: str):
         payload = []
         command = self.createCommand(StateOperations.DEL,key,payload)
         return await self.executeCommand(command)
     
-    async def hdel(self,htable,key):
-        payload = [key]
+    async def hdel(self,htable: str,keys: List[str]):
+        payload = keys
         command = self.createCommand(StateOperations.HDEL,htable,payload)
         return await self.executeCommand(command)
     
-    async def hexists(self,htable,key):
+    async def hexists(self,htable: str,key: str):
         payload = [key]
         command = self.createCommand(StateOperations.HEXISTS,htable,payload)
         return await self.executeCommand(command)
     
-    async def hgetall(self,htable):
+    async def hgetall(self,htable: str):
         payload = []
         command = self.createCommand(StateOperations.HGETALL,htable,payload)
         response = await self.executeCommand(command)
         result = {}
         for i in range(0,response.__len__(),2):
             result[response[i]] = response[i + 1]
         
         return result
     
-    async def hmget(self,htable,keys):
+    async def hmget(self,htable: str,keys: List[str]):
         command = self.createCommand(StateOperations.HMGET,htable,keys)
         response = await self.executeCommand(command)
         result = []
         for i in range(0,response.__len__()):
             result.append(response[i])
         
         return result
     
-    async def hvals(self,htable):
+    async def hvals(self,htable: str):
         payload = []
         command = self.createCommand(StateOperations.HVALS,htable,payload)
         response = await self.executeCommand(command)
         result = []
         for i in range(0,response.__len__()):
             result.append(response[i])
         
         return result
     
-    async def hget(self,htable,key):
+    async def hget(self,htable: str,key: str):
         payload = [key]
         command = self.createCommand(StateOperations.HGET,htable,payload)
         result = await self.executeCommand(command)
         return result
     
-    async def hset(self,htable,keyValuePairs):
+    async def hset(self,htable: str,keyValuePairs: Dict[str,str]):
         payload = []
         keys = self.bridge.getObjectKeys(keyValuePairs)
         for i in range(0,keys.__len__()):
             payload.append(keys[i])
             payload.append(keyValuePairs[keys[i]])
         
         command = self.createCommand(StateOperations.HSET,htable,payload)
         return await self.executeCommand(command)
     
-    async def hincrby(self,htable,key,value):
+    async def hincrby(self,htable: str,key: str,value: int):
         payload = [key,self.bridge.jsonStringify(value)]
         command = self.createCommand(StateOperations.HINCRBY,htable,payload)
         return await self.executeCommand(command)
     
-    async def hlen(self,htable):
+    async def hlen(self,htable: str):
         payload = []
         command = self.createCommand(StateOperations.HLEN,htable,payload)
         return await self.executeCommand(command)
     
-    async def hscan(self,htable,cursor,pattern,count):
+    async def hscan(self,htable: str,cursor: str,pattern: str,count: int):
         payload = [cursor,"MATCH",pattern,"COUNT",self.bridge.jsonStringify(count)]
         command = self.createCommand(StateOperations.HSCAN,htable,payload)
         return await self.executeCommand(command)
     
-    async def rpush(self,list,value):
+    async def rpush(self,list: str,value: T):
         payload = [self.bridge.jsonStringify(value)]
         command = self.createCommand(StateOperations.RPUSH,list,payload)
         return await self.executeCommand(command)
     
-    async def rpop(self,list,count = 1):
+    async def rpop(self,list: str,count: int = 1):
         args = [self.bridge.jsonStringify(count)]
         command = self.createCommand(StateOperations.RPOP,list,args)
         response = await self.executeCommand(command)
         result = self.parseResponse(response)
         return result
     
-    async def lpush(self,list,value):
+    async def lpush(self,list: str,value: T):
         payload = [self.bridge.jsonStringify(value)]
         command = self.createCommand(StateOperations.LPUSH,list,payload)
         return await self.executeCommand(command)
     
-    async def lpop(self,list,count = 1):
+    async def lpop(self,list: str,count: int = 1):
         args = [self.bridge.jsonStringify(count)]
         command = self.createCommand(StateOperations.LPOP,list,args)
         response = await self.executeCommand(command)
         result = self.parseResponse(response)
         return result
     
-    async def lrem(self,list,value,count = 0):
+    async def lrem(self,list: str,value: T,count: int = 0):
         args = [self.bridge.jsonStringify(count),self.bridge.jsonStringify(value)]
         command = self.createCommand(StateOperations.LREM,list,args)
         return await self.executeCommand(command)
     
-    async def llen(self,list):
+    async def llen(self,list: str):
         payload = []
         command = self.createCommand(StateOperations.LLEN,list,payload)
         return await self.executeCommand(command)
     
-    async def lrange(self,list,startPos = 0,endPos = -1):
+    async def lrange(self,list: str,startPos: int = 0,endPos: int = -1):
         args = [self.bridge.jsonStringify(startPos),self.bridge.jsonStringify(endPos)]
         command = self.createCommand(StateOperations.LRANGE,list,args)
         response = await self.executeCommand(command)
         result = self.parseResponse(response)
         return result
     
-    async def ltrim(self,list,startPos,endPos):
+    async def ltrim(self,list: str,startPos: int,endPos: int):
         args = [self.bridge.jsonStringify(startPos),self.bridge.jsonStringify(endPos)]
         command = self.createCommand(StateOperations.LTRIM,list,args)
         response = await self.executeCommand(command)
         return response
     
-    async def linsert(self,list,before,pivot,value):
+    async def linsert(self,list: str,before: bool,pivot: T,value: T):
         direction = "AFTER"
         if before is True:
             direction = "BEFORE"
         
         args = [direction,self.bridge.jsonStringify(pivot),self.bridge.jsonStringify(value)]
         command = self.createCommand(StateOperations.LINSERT,list,args)
         response = await self.executeCommand(command)
         return response
     
-    async def lindex(self,list,position):
+    async def lindex(self,list: str,position: int):
         args = [self.bridge.jsonStringify(position)]
         command = self.createCommand(StateOperations.LINDEX,list,args)
         response = await self.executeCommand(command)
         return self.bridge.jsonParse(response)
     
-    async def lset(self,list,position,value):
+    async def lset(self,list: str,position: int,value: T):
         args = [self.bridge.jsonStringify(position),self.bridge.jsonStringify(value)]
         command = self.createCommand(StateOperations.LSET,list,args)
         return await self.executeCommand(command)
     
-    async def incrby(self,key,value):
+    async def incrby(self,key: str,value: int):
         args = [self.bridge.jsonStringify(value)]
         command = self.createCommand(StateOperations.INCRBY,key,args)
         response = await self.executeCommand(command)
         return self.bridge.jsonParse(response)
     
-    async def decrby(self,key,value):
+    async def decrby(self,key: str,value: int):
         args = [self.bridge.jsonStringify(value)]
         command = self.createCommand(StateOperations.DECRBY,key,args)
         response = await self.executeCommand(command)
         return self.bridge.jsonParse(response)
     
-    async def expire(self,key,seconds,option = None):
+    async def expire(self,key: str,seconds: int,option: ExpireOptions = None):
         args = [self.bridge.jsonStringify(seconds)]
         if option is not None:
             args.append(option)
         
         command = self.createCommand(StateOperations.EXPIRE,key,args)
         return await self.executeCommand(command)
     
-    def parseResponse(self,response):
+    def parseResponse(self,response: List[str]):
         result = []
         if response is not None:
             for i in range(0,response.__len__()):
                 result.append(self.bridge.jsonParse(response[i]))
             
         
         return result
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/state/stateCommand.py` & `nerualpha-5.0.0/src/nerualpha/providers/state/stateCommand.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @dataclass
 class StateCommand(IStateCommand):
     args: List[str]
     key: str
     namespace: str
     operation: str
-    def __init__(self,operation,namespace,key,args):
+    def __init__(self,operation: str,namespace: str,key: str,args: List[str]):
         self.operation = operation
         self.namespace = namespace
         self.key = key
         self.args = args
     
     def reprJSON(self):
         result = {}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/state/stateOperations.py` & `nerualpha-5.0.0/src/nerualpha/providers/state/stateOperations.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IConversation.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/IConversation.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,84 +31,84 @@
 from nerualpha.providers.voice.contracts.earmuffResponseBody import EarmuffResponseBody
 from nerualpha.providers.voice.contracts.muteResponseBody import MuteResponseBody
 
 
 #interface
 class IConversation(ABC):
     @abstractmethod
-    def acceptInboundCall(self,event):
+    def acceptInboundCall(self,event: IAcceptInboundCallEvent):
         pass
     @abstractmethod
-    def inviteMember(self,name,channel):
+    def inviteMember(self,name: str,channel: IChannel):
         pass
     @abstractmethod
-    def onConversationCreated(self,callback):
+    def onConversationCreated(self,callback: str):
         pass
     @abstractmethod
-    def addUser(self,name):
+    def addUser(self,name: str):
         pass
     @abstractmethod
-    def transferMember(self,userId,legId):
+    def transferMember(self,userId: str,legId: str):
         pass
     @abstractmethod
-    def deleteMember(self,memberId):
+    def deleteMember(self,memberId: str):
         pass
     @abstractmethod
-    def sayText(self,body,to = None):
+    def sayText(self,body: ISayTextBody,to: str = None):
         pass
     @abstractmethod
-    def sayStop(self,sayId,to = None):
+    def sayStop(self,sayId: str,to: str = None):
         pass
     @abstractmethod
-    def playStream(self,body,to = None):
+    def playStream(self,body: IPlayStreamBody,to: str = None):
         pass
     @abstractmethod
-    def playStop(self,playId,to = None):
+    def playStop(self,playId: str,to: str = None):
         pass
     @abstractmethod
-    def earmuffOn(self,to,from_ = None):
+    def earmuffOn(self,to: str,from_: str = None):
         pass
     @abstractmethod
-    def earmuffOff(self,to,from_ = None):
+    def earmuffOff(self,to: str,from_: str = None):
         pass
     @abstractmethod
-    def muteOn(self,to,from_ = None):
+    def muteOn(self,to: str,from_: str = None):
         pass
     @abstractmethod
-    def muteOff(self,to,from_ = None):
+    def muteOff(self,to: str,from_: str = None):
         pass
     @abstractmethod
-    def listenForEvents(self,callback,filters):
+    def listenForEvents(self,callback: str,filters: List[IFilter]):
         pass
     @abstractmethod
-    def onSay(self,callback):
+    def onSay(self,callback: str):
         pass
     @abstractmethod
-    def onPlay(self,callback):
+    def onPlay(self,callback: str):
         pass
     @abstractmethod
-    def onSayStop(self,callback):
+    def onSayStop(self,callback: str):
         pass
     @abstractmethod
-    def onPlayStop(self,callback):
+    def onPlayStop(self,callback: str):
         pass
     @abstractmethod
-    def onSayDone(self,callback):
+    def onSayDone(self,callback: str):
         pass
     @abstractmethod
-    def onPlayDone(self,callback):
+    def onPlayDone(self,callback: str):
         pass
     @abstractmethod
-    def onLegStatusUpdate(self,callback):
+    def onLegStatusUpdate(self,callback: str):
         pass
     @abstractmethod
-    def onMemberJoined(self,callback,memberName = None):
+    def onMemberJoined(self,callback: str,memberName: str = None):
         pass
     @abstractmethod
-    def onMemberInvited(self,callback,memberName = None):
+    def onMemberInvited(self,callback: str,memberName: str = None):
         pass
     @abstractmethod
-    def onMemberLeft(self,callback,memberName = None):
+    def onMemberLeft(self,callback: str,memberName: str = None):
         pass
     @abstractmethod
-    def onDTMF(self,callback):
+    def onDTMF(self,callback: str):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/IVoice.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/IVoice.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 from nerualpha.providers.vonageAPI.contracts.invokePayload import InvokePayload
 from nerualpha.providers.voice.contracts.vapiCreateCallPayload import VapiCreateCallPayload
 from nerualpha.providers.voice.conversation import Conversation
 from nerualpha.providers.voice.contracts.IVapiEventParams import IVapiEventParams
 from nerualpha.providers.voice.contracts.IChannelPhoneEndpoint import IChannelPhoneEndpoint
 from nerualpha.providers.voice.contracts.vapiCreateCallResponse import VapiCreateCallResponse
 from nerualpha.providers.voice.contracts.IVapiCreateCallOptions import IVapiCreateCallOptions
-
+T = TypeVar('T')
 
 #interface
 class IVoice(ABC):
     @abstractmethod
-    def onInboundCall(self,callback,to,from_ = None):
+    def onInboundCall(self,callback: str,to: IChannelPhoneEndpoint,from_: IChannelPhoneEndpoint = None):
         pass
     @abstractmethod
-    def createConversation(self,name = None,displayName = None):
+    def createConversation(self,name: str = None,displayName: str = None):
         pass
     @abstractmethod
-    def onVapiAnswer(self,callback):
+    def onVapiAnswer(self,callback: str):
         pass
     @abstractmethod
-    def onVapiEvent(self,params):
+    def onVapiEvent(self,params: IVapiEventParams):
         pass
     @abstractmethod
-    def vapiCreateCall(self,from_,to,ncco,options = None):
+    def vapiCreateCall(self,from_: IChannelPhoneEndpoint,to: List[IChannelPhoneEndpoint],ncco: List[Dict[str,object]],options: IVapiCreateCallOptions = None):
         pass
     @abstractmethod
-    def uploadNCCO(self,uuid,ncco):
+    def uploadNCCO(self,uuid: str,ncco: T):
         pass
     @abstractmethod
-    def getConversation(self,id):
+    def getConversation(self,id: str):
         pass
     @abstractmethod
-    def getCallRecording(self,recordingUrl):
+    def getCallRecording(self,recordingUrl: str):
         pass
     @abstractmethod
-    def uploadCallRecording(self,recordingUrl,assetsPath):
+    def uploadCallRecording(self,recordingUrl: str,assetsPath: str):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/IChannel.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/IChannel.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/Link.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/muteResponseBody.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 
 @dataclass
-class Link:
-    href: str = None
+class MuteResponseBody:
+    rtc_id: str
     def __init__(self):
         pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/acceptInboundCallBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallEndpoint.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/acceptInboundCallEndpoint.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallEvent.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/acceptInboundCallEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/acceptInboundCallPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/acceptInboundCallPayload.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 @dataclass
 class AcceptInboundCallPayload(IAcceptInboundCallPayload):
     media: IMedia
     state: str
     channel: IChannel
     knocking_id: str
     user: IUser
-    def __init__(self,userId,knockingId,channel,media):
+    def __init__(self,userId: str,knockingId: str,channel: IChannel,media: IMedia):
         user = User()
         user.id = userId
         self.user = user
         self.knocking_id = knockingId
         self.channel = channel
         self.state = MemberStates.Joined
         self.media = media
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/addUserPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/addUserPayload.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from nerualpha.providers.voice.contracts.IAddUserPayload import IAddUserPayload
 
 @dataclass
 class AddUserPayload(IAddUserPayload):
     display_name: str
     name: str
-    def __init__(self,name):
+    def __init__(self,name: str):
         self.name = name
         self.display_name = name
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/addUserResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/addUserResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSayResponseBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/audioSayResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSayStopResponseBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/audioSayStopResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/audioSettings.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/audioSettings.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nerualpha.providers.voice.contracts.IAudioSettings import IAudioSettings
 
 @dataclass
 class AudioSettings(IAudioSettings):
     muted: bool
     earmuffed: bool
     enabled: bool
-    def __init__(self,enabled,earmuffed,muted):
+    def __init__(self,enabled: bool,earmuffed: bool,muted: bool):
         self.enabled = enabled
         self.earmuffed = earmuffed
         self.muted = muted
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channel.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channel.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelAppEndpoint.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channelAppEndpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nerualpha.providers.voice.contracts.IChannelEndpoint import IChannelEndpoint
 from nerualpha.providers.voice.csChannelTypes import CSChannelTypes
 
 @dataclass
 class ChannelAppEndpoint(IChannelEndpoint):
     user: str
     type_: str
-    def __init__(self,user):
+    def __init__(self,user: str):
         self.user = user
         self.type_ = CSChannelTypes.APP
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelPhoneEndpoint.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channelPhoneEndpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nerualpha.providers.voice.contracts.IChannelPhoneEndpoint import IChannelPhoneEndpoint
 from nerualpha.providers.voice.csChannelTypes import CSChannelTypes
 
 @dataclass
 class ChannelPhoneEndpoint(IChannelPhoneEndpoint):
     number: str
     type_: str
-    def __init__(self,number):
+    def __init__(self,number: str):
         self.number = number
         self.type_ = CSChannelTypes.PHONE
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelSIPEndpoint.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channelSIPEndpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @dataclass
 class ChannelSIPEndpoint(IChannelSIPEndpoint):
     headers: Dict[str,str]
     uri: str
     type_: str
     username: str = None
     password: str = None
-    def __init__(self,uri,headers,username = None,password = None):
+    def __init__(self,uri: str,headers: Dict[str,str],username: str = None,password: str = None):
         self.type_ = CSChannelTypes.SIP
         self.uri = uri
         self.headers = headers
         if username is not None:
             self.username = username
         
         if password is not None:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/channelVBCEndpoint.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/channelVBCEndpoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nerualpha.providers.voice.contracts.IChannelVBCEndpoint import IChannelVBCEndpoint
 from nerualpha.providers.voice.csChannelTypes import CSChannelTypes
 
 @dataclass
 class ChannelVBCEndpoint(IChannelVBCEndpoint):
     extension: str
     type_: str
-    def __init__(self,extension):
+    def __init__(self,extension: str):
         self.type_ = CSChannelTypes.VBC
         self.extension = extension
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/conversationPayloadWithCallback.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/conversationPayloadWithCallback.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nerualpha.providers.voice.contracts.IConversationPayloadWithCallback import IConversationPayloadWithCallback
 from nerualpha.session.IWrappedCallback import IWrappedCallback
 
 @dataclass
 class ConversationPayloadWithCallback(IConversationPayloadWithCallback):
     conversationId: str
     callback: IWrappedCallback
-    def __init__(self,callback,conversationId):
+    def __init__(self,callback: IWrappedCallback,conversationId: str):
         self.callback = callback
         self.conversationId = conversationId
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/conversationTimestamp.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/conversationTimestamp.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createConversationPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/createConversationPayload.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from nerualpha.providers.voice.contracts.ICreateConversationPayload import ICreateConversationPayload
 
 @dataclass
 class CreateConversationPayload(ICreateConversationPayload):
     display_name: str
     name: str
-    def __init__(self,name,displayName):
+    def __init__(self,name: str,displayName: str):
         self.name = name
         self.display_name = displayName
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createConversationResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/createConversationResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/createUserPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/createUserPayload.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @dataclass
 class CreateUserPayload(ICreateUserPayload):
     display_name: str
     name: str
     image_url: str = None
     channels: object = None
-    def __init__(self,name,display_name,image_url = None,channels = None):
+    def __init__(self,name: str,display_name: str,image_url: str = None,channels: object = None):
         self.name = name
         self.display_name = display_name
         self.image_url = image_url
         self.channels = channels
     
     def reprJSON(self):
         result = {}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/deleteMemberPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/deleteMemberPayload.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nerualpha.providers.voice.contracts.IReason import IReason
 from nerualpha.providers.voice.memberStates import MemberStates
 
 @dataclass
 class DeleteMemberPayload(IDeleteMemberPayload):
     reason: IReason
     state: str
-    def __init__(self,reason):
+    def __init__(self,reason: IReason):
         self.state = MemberStates.Left
         self.reason = reason
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/earmuffPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/earmuffPayload.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nerualpha.providers.voice.csEvents import CSEvents
 
 @dataclass
 class EarmuffPayload(IEarmuffPayload):
     to: str
     type_: str
     from_: str = None
-    def __init__(self,enable,to,from_ = None):
+    def __init__(self,enable: bool,to: str,from_: str = None):
         if enable:
             self.type_ = CSEvents.EarmuffOn
         
         else: 
             self.type_ = CSEvents.EarmuffOff
         
         self.to = to
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/earmuffResponseBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/earmuffResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/embeddedUsers.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/embeddedUsers.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/eventEmbedded.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/eventEmbedded.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/eventResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/eventResponse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.voice.contracts.Link import Link
 from nerualpha.providers.voice.contracts.eventEmbedded import EventEmbedded
-
+T = TypeVar('T')
 T = TypeVar("T")
 
 @dataclass
 class EventResponse(Generic[T]):
     _links: Link
     timestamp: str
     id: int
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/getUsersResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/getUsersResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/inviteMemberPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/inviteMemberPayload.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @dataclass
 class InviteMemberPayload(IInviteMemberPayload):
     channel: IChannel
     state: str
     action: str
     user: IUser
-    def __init__(self,userName,channel):
+    def __init__(self,userName: str,channel: IChannel):
         user = User()
         user.name = userName
         self.user = user
         self.action = MemberActions.Join
         self.state = MemberStates.Invited
         self.channel = channel
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/leg.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/leg.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/media.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/media.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nerualpha.providers.voice.contracts.IMedia import IMedia
 from nerualpha.providers.voice.contracts.IAudioSettings import IAudioSettings
 
 @dataclass
 class Media(IMedia):
     audio: bool
     audio_settings: IAudioSettings
-    def __init__(self,settings,audio):
+    def __init__(self,settings: IAudioSettings,audio: bool):
         self.audio_settings = settings
         self.audio = audio
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/member.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/member.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/memberResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/memberResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/memberTimestamp.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/memberTimestamp.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/mutePayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/mutePayload.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nerualpha.providers.voice.csEvents import CSEvents
 
 @dataclass
 class MutePayload(IMutePayload):
     to: str
     type_: str
     from_: str = None
-    def __init__(self,enable,to,from_ = None):
+    def __init__(self,enable: bool,to: str,from_: str = None):
         if enable:
             self.type_ = CSEvents.MuteOn
         
         else: 
             self.type_ = CSEvents.MuteOff
         
         self.to = to
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/muteResponseBody.py` & `nerualpha-5.0.0/src/nerualpha/smokes/schedulerTestPayload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 
 @dataclass
-class MuteResponseBody:
-    rtc_id: str
+class SchedulerTestPayload:
+    text: str = field(default = "test payload")
     def __init__(self):
         pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/onInboundCallPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/onInboundCallPayload.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from nerualpha.providers.voice.contracts.IChannelPhoneEndpoint import IChannelPhoneEndpoint
 
 @dataclass
 class OnInboundCallPayload(IOnInboundCallPayload):
     to: IChannelPhoneEndpoint
     callback: IWrappedCallback
     from_: IChannelPhoneEndpoint = None
-    def __init__(self,callback,to,from_ = None):
+    def __init__(self,callback: IWrappedCallback,to: IChannelPhoneEndpoint,from_: IChannelPhoneEndpoint = None):
         self.callback = callback
         self.to = to
         if from_ is not None:
             self.from_ = from_
         
     
     def reprJSON(self):
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStopBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStopBody.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.voice.contracts.IPlayStopBody import IPlayStopBody
 
 @dataclass
 class PlayStopBody(IPlayStopBody):
     play_id: str
-    def __init__(self,playId):
+    def __init__(self,playId: str):
         self.play_id = playId
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStopPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStopPayload.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from nerualpha.providers.voice.contracts.playStopBody import PlayStopBody
 
 @dataclass
 class PlayStopPayload(IPlayStopPayload):
     body: IPlayStopBody
     type_: str
     to: str = None
-    def __init__(self,playId,to = None):
+    def __init__(self,playId: str,to: str = None):
         self.type_ = CSEvents.AudioPlayStop
         self.body = PlayStopBody(playId)
         if to is not None:
             self.to = to
         
     
     def reprJSON(self):
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStreamBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStreamPayload.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from nerualpha.providers.voice.contracts.IPlayStreamBody import IPlayStreamBody
 
 @dataclass
 class PlayStreamPayload(IPlayStreamPayload):
     body: IPlayStreamBody
     type_: str
     to: str = None
-    def __init__(self,body,to = None):
+    def __init__(self,body: IPlayStreamBody,to: str = None):
         self.type_ = CSEvents.AudioPlay
         self.body = body
         if to is not None:
             self.to = to
         
     
     def reprJSON(self):
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamResponseBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStreamResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/playStreamStopResponseBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/playStreamStopResponseBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/reason.py` & `nerualpha-5.0.0/src/nerualpha/services/jwt/acl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.providers.voice.contracts.IReason import IReason
+from nerualpha.services.jwt.IAcl import IAcl
 
 @dataclass
-class Reason(IReason):
-    text: str
-    code: str
-    def __init__(self,code,text):
-        self.code = code
-        self.text = text
-    
+class Acl(IAcl):
+    paths: Dict[str,Dict[str,object]]
+    def __init__(self):
+        pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/responseProperties.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/responseProperties.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayStopBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayStopBody.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.voice.contracts.ISayStopBody import ISayStopBody
 
 @dataclass
 class SayStopBody(ISayStopBody):
     say_id: str
-    def __init__(self,sayId):
+    def __init__(self,sayId: str):
         self.say_id = sayId
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayStopPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/reason.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.providers.voice.contracts.ISayStopPayload import ISayStopPayload
-from nerualpha.providers.voice.csEvents import CSEvents
-from nerualpha.providers.voice.contracts.ISayStopBody import ISayStopBody
-from nerualpha.providers.voice.contracts.sayStopBody import SayStopBody
+from nerualpha.providers.voice.contracts.IReason import IReason
 
 @dataclass
-class SayStopPayload(ISayStopPayload):
-    body: ISayStopBody
-    type_: str
-    to: str = None
-    def __init__(self,sayId,to = None):
-        self.type_ = CSEvents.AudioSayStop
-        self.body = SayStopBody(sayId)
-        if to is not None:
-            self.to = to
-        
+class Reason(IReason):
+    text: str
+    code: str
+    def __init__(self,code: str,text: str):
+        self.code = code
+        self.text = text
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextBody.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayTextBody.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextParams.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayTextParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/sayTextPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayTextPayload.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from nerualpha.providers.voice.contracts.ISayTextBody import ISayTextBody
 
 @dataclass
 class SayTextPayload(ISayTextPayload):
     body: ISayTextBody
     type_: str
     to: str = None
-    def __init__(self,body,to = None):
+    def __init__(self,body: ISayTextBody,to: str = None):
         self.type_ = CSEvents.AudioSay
         self.body = body
         if to is not None:
             self.to = to
         
     
     def reprJSON(self):
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/selfLink.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/selfLink.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/transferMemberPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/transferMemberPayload.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @dataclass
 class TransferMemberPayload(ITransferMemberPayload):
     user: IUser
     state: str
     channel: IChannel
     action: str
-    def __init__(self,userId,legId):
+    def __init__(self,userId: str,legId: str):
         self.action = MemberActions.Join
         self.channel = Channel()
         self.channel.id = legId
         self.channel.type_ = CSChannelTypes.PHONE
         self.state = MemberStates.Joined
         user = User()
         user.id = userId
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/updateUserPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/updateUserPayload.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @dataclass
 class UpdateUserPayload(IUpdateUserPayload):
     name: str = None
     display_name: str = None
     image_url: str = None
     channels: object = None
-    def __init__(self,name = None,display_name = None,image_url = None,channels = None):
+    def __init__(self,name: str = None,display_name: str = None,image_url: str = None,channels: object = None):
         self.name = name
         self.display_name = display_name
         self.image_url = image_url
         self.channels = channels
     
     def reprJSON(self):
         result = {}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/user.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/user.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userEmbedded.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/urlPayload.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.providers.voice.contracts.user import User
+from nerualpha.webhookEvents.IUrlPayload import IUrlPayload
 
 @dataclass
-class UserEmbedded:
-    user: User
+class UrlPayload(IUrlPayload):
+    url: str
     def __init__(self):
         pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/userResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userSummary.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/userSummary.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/userTimestamp.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/userTimestamp.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiAnswerCallBack.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiAnswerCallBack.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from nerualpha.providers.voice.contracts.IVapiAnswerCallBack import IVapiAnswerCallBack
 from nerualpha.session.IWrappedCallback import IWrappedCallback
 
 @dataclass
 class VapiAnswerCallBack(IVapiAnswerCallBack):
     callback: IWrappedCallback
-    def __init__(self,callback):
+    def __init__(self,callback: IWrappedCallback):
         self.callback = callback
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallOptions.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiCreateCallOptions.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiCreateCallPayload.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     ncco: List[Dict[str,object]]
     to: List[IChannelPhoneEndpoint]
     from_: IChannelPhoneEndpoint
     ringing_timer: int = None
     length_timer: int = None
     machine_detection: str = None
     random_from_number: bool = None
-    def __init__(self,from_,to,ncco,options = None):
+    def __init__(self,from_: IChannelPhoneEndpoint,to: List[IChannelPhoneEndpoint],ncco: List[Dict[str,object]],options: IVapiCreateCallOptions = None):
         self.from_ = from_
         self.to = to
         self.ncco = ncco
         if options is not None:
             if options.machineDetection is not None:
                 self.machine_detection = options.machineDetection
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiCreateCallResponse.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiCreateCallResponse.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiEventCallBackPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiEventCallBackPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/contracts/vapiEventParams.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/vapiEventParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/conversation.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/conversation.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,59 +49,59 @@
 class Conversation(IConversation):
     baseUrl: str
     vonageAPI: IVonageAPI
     session: ISession
     name: str
     id: str
     provider: str = field(default = "vonage-voice")
-    def __init__(self,id,session):
+    def __init__(self,id: str,session: ISession):
         self.id = id
         self.session = session
         self.vonageAPI = VonageAPI(self.session)
         self.baseUrl = "https://api.nexmo.com/v0.3"
     
-    def acceptInboundCall(self,event):
+    def acceptInboundCall(self,event: IAcceptInboundCallEvent):
         audioSettings = AudioSettings(True,False,False)
         media = Media(audioSettings,True)
         channel = Channel()
         channel.id = event.body.channel.id
         channel.type_ = event.body.channel.type_
         channel.to = event.body.channel.to
         channel.from_ = event.body.channel.from_
         payload = AcceptInboundCallPayload(event.body.user.id,event.from_,channel,media)
         url = f'{self.baseUrl}/conversations/{self.id}/members'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def inviteMember(self,name,channel):
+    def inviteMember(self,name: str,channel: IChannel):
         payload = InviteMemberPayload(name,channel)
         url = f'{self.baseUrl}/conversations/{self.id}/members'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def addUser(self,name):
+    def addUser(self,name: str):
         payload = AddUserPayload(name)
         url = f'{self.baseUrl}/users'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def transferMember(self,userId,legId):
+    def transferMember(self,userId: str,legId: str):
         payload = TransferMemberPayload(userId,legId)
         url = f'{self.baseUrl}/conversations/{self.id}/members'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def deleteMember(self,memberId):
+    def deleteMember(self,memberId: str):
         reason = Reason("123","leaving conversation")
         payload = DeleteMemberPayload(reason)
         url = f'{self.baseUrl}/conversations/{self.id}/members/{memberId}'
         method = f'PATCH'
         return self.vonageAPI.invoke(url,method,payload)
     
-    def sayText(self,body,to = None):
+    def sayText(self,body: ISayTextBody,to: str = None):
         if body.level is None:
             body.level = 1
         
         if body.loop is None:
             body.loop = 1
         
         if body.voice_name is None:
@@ -114,121 +114,121 @@
             body.ssml = False
         
         payload = SayTextPayload(body,to)
         method = "POST"
         url = f'{self.baseUrl}/conversations/{self.id}/events'
         return self.vonageAPI.invoke(url,method,payload)
     
-    def sayStop(self,sayId,to = None):
+    def sayStop(self,sayId: str,to: str = None):
         payload = SayStopPayload(sayId,to)
         url = f'{self.baseUrl}/conversations/{self.id}/events'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def playStream(self,body,to = None):
+    def playStream(self,body: IPlayStreamBody,to: str = None):
         if body.loop is None:
             body.loop = 1
         
         if body.level is None:
             body.level = 1
         
         payload = PlayStreamPayload(body,to)
         url = f'{self.baseUrl}/conversations/{self.id}/events'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def playStop(self,playId,to = None):
+    def playStop(self,playId: str,to: str = None):
         payload = PlayStopPayload(playId,to)
         url = f'{self.baseUrl}/conversations/{self.id}/events'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def earmuff(self,enable,to,from_ = None):
+    def earmuff(self,enable: bool,to: str,from_: str = None):
         payload = EarmuffPayload(enable,to,from_)
         url = f'{self.baseUrl}/conversations/{self.id}/events'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def earmuffOn(self,to,from_ = None):
+    def earmuffOn(self,to: str,from_: str = None):
         return self.earmuff(True,to,from_)
     
-    def earmuffOff(self,to,from_ = None):
+    def earmuffOff(self,to: str,from_: str = None):
         return self.earmuff(False,to,from_)
     
-    def mute(self,enable,to,from_ = None):
+    def mute(self,enable: bool,to: str,from_: str = None):
         payload = MutePayload(enable,to,from_)
         url = f'{self.baseUrl}/conversations/{self.id}/events'
         method = "POST"
         return self.vonageAPI.invoke(url,method,payload)
     
-    def muteOn(self,to,from_ = None):
+    def muteOn(self,to: str,from_: str = None):
         return self.mute(True,to,from_)
     
-    def muteOff(self,to,from_ = None):
+    def muteOff(self,to: str,from_: str = None):
         return self.mute(False,to,from_)
     
-    def listenForEvents(self,callback,filters):
+    def listenForEvents(self,callback: str,filters: List[IFilter]):
         payload = ConversationPayloadWithCallback(self.session.wrapCallback(callback,filters),self.id)
         action = ActionPayload(self.provider,VoiceActions.ConversationSubscribeEvent,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    def onConversationCreated(self,callback):
+    def onConversationCreated(self,callback: str):
         filters = [Filter("type","contains",[CSEvents.ConversationCreated]),Filter("body.name","contains",[self.name])]
         return self.listenForEvents(callback,filters)
     
-    def onSay(self,callback):
+    def onSay(self,callback: str):
         filters = [Filter("type","contains",[CSEvents.AudioSay]),Filter(f'conversation_id',f'contains',[self.id])]
         return self.listenForEvents(callback,filters)
     
-    def onPlay(self,callback):
+    def onPlay(self,callback: str):
         filters = [Filter("type","contains",[CSEvents.AudioPlay]),Filter("conversation_id","contains",[self.id])]
         return self.listenForEvents(callback,filters)
     
-    def onSayStop(self,callback):
+    def onSayStop(self,callback: str):
         filters = [Filter("type","contains",[CSEvents.AudioSayStop]),Filter(f'conversation_id',f'contains',[self.id])]
         return self.listenForEvents(callback,filters)
     
-    def onPlayStop(self,callback):
+    def onPlayStop(self,callback: str):
         filters = [Filter("type","contains",[CSEvents.AudioPlayStop]),Filter(f'conversation_id',f'contains',[self.id])]
         return self.listenForEvents(callback,filters)
     
-    def onSayDone(self,callback):
+    def onSayDone(self,callback: str):
         filters = [Filter("type","contains",[CSEvents.AudioSayDone]),Filter(f'conversation_id',f'contains',[self.id])]
         return self.listenForEvents(callback,filters)
     
-    def onPlayDone(self,callback):
+    def onPlayDone(self,callback: str):
         filters = [Filter("type","contains",[CSEvents.AudioPlayDone]),Filter(f'conversation_id',f'contains',[self.id])]
         return self.listenForEvents(callback,filters)
     
-    def onLegStatusUpdate(self,callback):
+    def onLegStatusUpdate(self,callback: str):
         filters = [Filter("type","contains",[CSEvents.LegStatusUpdate]),Filter(f'conversation_id',f'contains',[self.id])]
         return self.listenForEvents(callback,filters)
     
-    def onMemberJoined(self,callback,memberName = None):
+    def onMemberJoined(self,callback: str,memberName: str = None):
         filters = [Filter("type","contains",[CSEvents.MemberJoined]),Filter(f'conversation_id',f'contains',[self.id])]
         if memberName is not None:
             filters.append(Filter(f'body.user.name',f'contains',[memberName]))
         
         return self.listenForEvents(callback,filters)
     
-    def onMemberInvited(self,callback,memberName = None):
+    def onMemberInvited(self,callback: str,memberName: str = None):
         filters = [Filter("type","contains",[CSEvents.MemberInvited]),Filter(f'conversation_id',f'contains',[self.id])]
         if memberName is not None:
             filters.append(Filter("body.user.name","contains",[memberName]))
         
         return self.listenForEvents(callback,filters)
     
-    def onMemberLeft(self,callback,memberName = None):
+    def onMemberLeft(self,callback: str,memberName: str = None):
         filters = [Filter("type","contains",[CSEvents.MemberLeft]),Filter(f'conversation_id',f'contains',[self.id])]
         if memberName is not None:
             filters.append(Filter("body.user.name","contains",[memberName]))
         
         return self.listenForEvents(callback,filters)
     
-    def onDTMF(self,callback):
+    def onDTMF(self,callback: str):
         filters = [Filter("type","contains",[CSEvents.AudioDTMF]),Filter(f'conversation_id',f'contains',[self.id])]
         return self.listenForEvents(callback,filters)
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/csEvents.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/csEvents.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/users.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
 @dataclass
 class Users(IUsers):
     bridge: IBridge
     baseUrl: str
     vonageAPI: IVonageAPI
     session: ISession
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.session = session
         self.bridge = session.bridge
         self.vonageAPI = VonageAPI(self.session)
         self.baseUrl = "https://api.nexmo.com/v0.3"
     
-    def getUsers(self,page_size = None,order = None,pageUrl = None):
+    def getUsers(self,page_size: int = None,order: str = None,pageUrl: str = None):
         url = ""
         if pageUrl is not None:
             url = pageUrl
         
         else: 
             options = {}
             if page_size:
@@ -40,35 +40,35 @@
                 options["order"] = order
             
             url = self.buildUrl(f'{self.baseUrl}/users',options)
         
         method = "GET"
         return self.vonageAPI.invoke(url,method,None)
     
-    def getUser(self,user_id):
+    def getUser(self,user_id: String):
         url = f'{self.baseUrl}/users/{user_id}'
         method = "GET"
         return self.vonageAPI.invoke(url,method,None)
     
-    def createUser(self,createUserPayload):
+    def createUser(self,createUserPayload: CreateUserPayload):
         url = f'{self.baseUrl}/users'
         method = "POST"
         return self.vonageAPI.invoke(url,method,createUserPayload)
     
-    def updateUser(self,user_id,updateUserPayload):
+    def updateUser(self,user_id: str,updateUserPayload: UpdateUserPayload):
         url = f'{self.baseUrl}/users/{user_id}'
         method = "PATCH"
         return self.vonageAPI.invoke(url,method,updateUserPayload)
     
-    def deleteUser(self,user_id):
+    def deleteUser(self,user_id: String):
         url = f'{self.baseUrl}/users/{user_id}'
         method = "DELETE"
         return self.vonageAPI.invoke(url,method,None)
     
-    def buildUrl(self,baseUrl,options):
+    def buildUrl(self,baseUrl: str,options: Dict[str,object]):
         keys = self.bridge.getObjectKeys(options)
         queryString = ""
         for i in range(0,keys.__len__()):
             key = keys[i]
             value = options[key]
             queryString += f'{key}={value}'
             if i + 1 < keys.__len__():
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/voice/voice.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,44 +25,44 @@
 from nerualpha.providers.voice.contracts.vapiCreateCallResponse import VapiCreateCallResponse
 from nerualpha.providers.voice.contracts.IVapiCreateCallOptions import IVapiCreateCallOptions
 from nerualpha.request.requestParams import RequestParams
 from nerualpha.request.responseTypes import ResponseTypes
 from nerualpha.services.jwt.createVonageTokenParams import CreateVonageTokenParams
 from nerualpha.providers.assets.assets import Assets
 from nerualpha.request.requestMethods import RequestMethods
-
+T = TypeVar('T')
 @dataclass
 class Voice(IVoice):
     bridge: IBridge
     assetsAPI: Assets
     vonageApi: IVonageAPI
     session: ISession
     provider: str = field(default = "vonage-voice")
     regionURL: str = field(default = "https://api.nexmo.com")
-    def __init__(self,session,regionURL = None):
+    def __init__(self,session: ISession,regionURL: str = None):
         self.session = session
         self.bridge = session.bridge
         self.assetsAPI = Assets(session)
         self.vonageApi = VonageAPI(self.session)
         if regionURL is not None:
             self.regionURL = regionURL
         
     
-    def onInboundCall(self,callback,to,from_ = None):
+    def onInboundCall(self,callback: str,to: IChannelPhoneEndpoint,from_: IChannelPhoneEndpoint = None):
         if to.type_ is None:
             to.type_ = "phone"
         
         if from_ is not None and from_.type_ is None:
             from_.type_ = "phone"
         
         payload = OnInboundCallPayload(self.session.wrapCallback(callback,[]),to,from_)
         action = ActionPayload(self.provider,VoiceActions.ConversationSubscribeInboundCall,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    async def createConversation(self,name = None,displayName = None):
+    async def createConversation(self,name: str = None,displayName: str = None):
         conversationName = name
         conversationDisplayName = displayName
         if name is None:
             conversationId = self.bridge.substring(self.session.createUUID(),0,5)
             conversationName = f'name_cs_{conversationId}'
         
         if displayName is None:
@@ -70,60 +70,60 @@
         
         payload = CreateConversationPayload(conversationName,conversationDisplayName)
         url = "https://api.nexmo.com/v0.3/conversations"
         method = RequestMethods.POST
         res = await self.vonageApi.invoke(url,method,payload).execute()
         return Conversation(res.id,self.session)
     
-    def onVapiAnswer(self,callback):
+    def onVapiAnswer(self,callback: str):
         payload = VapiAnswerCallBack(self.session.wrapCallback(callback,[]))
         action = ActionPayload(self.provider,VoiceActions.VapiSubscribeInboundCall,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    def onVapiEvent(self,params):
+    def onVapiEvent(self,params: IVapiEventParams):
         payload = VapiEventCallBackPayload()
         payload.callback = self.session.wrapCallback(params.callback,[])
         if params.conversationID is None and params.vapiUUID is None:
             raise Exception("Either conversationID or vapiUUID is required")
         
         if params.vapiUUID is not None:
             payload.vapiID = params.vapiUUID
         
         elif params.conversationID is not None:
             payload.conversationID = params.conversationID
         
         action = ActionPayload(self.provider,VoiceActions.VapiSubscribeEvent,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    def vapiCreateCall(self,from_,to,ncco,options = None):
+    def vapiCreateCall(self,from_: IChannelPhoneEndpoint,to: List[IChannelPhoneEndpoint],ncco: List[Dict[str,object]],options: IVapiCreateCallOptions = None):
         vapiCreateCallPayload = VapiCreateCallPayload(from_,to,ncco,options)
         method = RequestMethods.POST
         return self.vonageApi.invoke(f'{self.regionURL}/v1/calls',method,vapiCreateCallPayload)
     
-    def uploadNCCO(self,uuid,ncco):
+    def uploadNCCO(self,uuid: str,ncco: T):
         method = RequestMethods.PUT
         return self.vonageApi.invoke(f'{self.regionURL}/v1/calls/{uuid}',method,ncco)
     
-    def getConversation(self,id):
+    def getConversation(self,id: str):
         return Conversation(id,self.session)
     
-    async def getCallRecording(self,recordingUrl):
+    async def getCallRecording(self,recordingUrl: str):
         params = RequestParams()
         params.method = RequestMethods.GET
         params.url = recordingUrl
         createVonageTokenParams = CreateVonageTokenParams()
         createVonageTokenParams.exp = self.bridge.getSystemTime() + 60 * 60
         token = self.session.jwt.createVonageToken(createVonageTokenParams)
         headers = {}
         headers["Authorization"] = f'Bearer {token}'
         params.headers = headers
         params.responseType = ResponseTypes.STREAM
         return await self.bridge.request(params)
     
-    async def uploadCallRecording(self,recordingUrl,assetsPath):
+    async def uploadCallRecording(self,recordingUrl: str,assetsPath: str):
         stream = await self.getCallRecording(recordingUrl)
         pathObject = self.bridge.parsePath(assetsPath)
         data = [stream]
         fileNames = [pathObject.base]
         await self.assetsAPI.uploadData(data,pathObject.dir,fileNames).execute()
     
     def reprJSON(self):
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/importPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/importPayload.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.vonageAI.contracts.IImportPayload import IImportPayload
 
 @dataclass
 class ImportPayload(IImportPayload):
     modelAsset: str
-    def __init__(self,modelAsset):
+    def __init__(self,modelAsset: str):
         self.modelAsset = modelAsset
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/vonageAiAnalyzePayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/vonageAiAnalyzePayload.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nerualpha.providers.vonageAI.contracts.IVonageAiAnalyzePayload import IVonageAiAnalyzePayload
 from nerualpha.session.IWrappedCallback import IWrappedCallback
 
 @dataclass
 class VonageAiAnalyzePayload(IVonageAiAnalyzePayload):
     callback: IWrappedCallback
     analyze: str
-    def __init__(self,analyze,callback):
+    def __init__(self,analyze: str,callback: IWrappedCallback):
         self.analyze = analyze
         self.callback = callback
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/contracts/vonageAiImportModelPayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/vonageAI/contracts/vonageAiImportModelPayload.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nerualpha.session.IWrappedCallback import IWrappedCallback
 from nerualpha.providers.vonageAI.contracts.IImportPayload import IImportPayload
 
 @dataclass
 class VonageAiImportModelPayload(IVonageAiImportModelPayload):
     import_: IImportPayload
     callback: IWrappedCallback
-    def __init__(self,importPayload,callback):
+    def __init__(self,importPayload: IImportPayload,callback: IWrappedCallback):
         self.import_ = importPayload
         self.callback = callback
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAI/vonageAI.py` & `nerualpha-5.0.0/src/nerualpha/providers/vonageAI/vonageAI.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 from nerualpha.providers.vonageAI.contracts.vonageAiImportModelPayload import VonageAiImportModelPayload
 from nerualpha.session.IPayloadWithCallback import IPayloadWithCallback
 
 @dataclass
 class VonageAI(IVonageAI):
     session: ISession
     provider: str = field(default = "vonage-overai")
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.session = session
     
-    def analyze(self,analyze,callback):
+    def analyze(self,analyze: str,callback: str):
         payload = VonageAiAnalyzePayload(analyze,self.session.wrapCallback(callback,[]))
         action = ActionPayload(self.provider,VonageAIActions.Analyze,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
-    def importModel(self,modelAssetName,callback):
+    def importModel(self,modelAssetName: str,callback: str):
         modelAsset = ImportPayload(modelAssetName)
         wrappedCallback = self.session.wrapCallback(callback,[])
         payload = VonageAiImportModelPayload(modelAsset,wrappedCallback)
         action = ActionPayload(self.provider,VonageAIActions.ImportModel,payload)
         return RequestInterfaceForCallbacks(self.session,action)
     
     def reprJSON(self):
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/contracts/invokePayload.py` & `nerualpha-5.0.0/src/nerualpha/providers/vonageAPI/contracts/invokePayload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.providers.vonageAPI.contracts.IInvokePayload import IInvokePayload
-
+T = TypeVar('T')
 T = TypeVar("T")
 
 @dataclass
 class InvokePayload(IInvokePayload,Generic[T]):
     body: T
     method: str
     url: str
-    def __init__(self,url,method,body):
+    def __init__(self,url: str,method: str,body: T):
         self.url = url
         self.method = method
         self.body = body
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/providers/vonageAPI/vonageAPI.py` & `nerualpha-5.0.0/src/nerualpha/providers/vonageAPI/vonageAPI.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 from nerualpha.session.requestInterface import RequestInterface
 from nerualpha.providers.vonageAPI.vonageAPIActions import VonageAPIActions
 from nerualpha.session.actionPayload import ActionPayload
 from nerualpha.providers.vonageAPI.IVonageAPI import IVonageAPI
 from nerualpha.session.ISession import ISession
 from nerualpha.providers.vonageAPI.contracts.invokePayload import InvokePayload
-
+T = TypeVar('T')
+K = TypeVar('K')
 @dataclass
 class VonageAPI(IVonageAPI):
     session: ISession
     provider: str = field(default = "vonage-api")
-    def __init__(self,session):
+    def __init__(self,session: ISession):
         self.session = session
     
-    def invoke(self,url,method,body):
+    def invoke(self,url: str,method: str,body: T):
         payload = InvokePayload(url,method,body)
         action = ActionPayload(self.provider,VonageAPIActions.Invoke,payload)
         return RequestInterface(self.session,action)
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/request/formDataObject.py` & `nerualpha-5.0.0/src/nerualpha/request/formDataObject.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/request/request.py` & `nerualpha-5.0.0/src/nerualpha/request/request.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/request/requestParams.py` & `nerualpha-5.0.0/src/nerualpha/request/requestParams.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.request.IRequestParams import IRequestParams
 from nerualpha.request.responseTypes import ResponseTypes
-
+T = TypeVar('T')
 T = TypeVar("T")
 
 @dataclass
 class RequestParams(IRequestParams,Generic[T]):
     url: str
     method: str
     data: T = None
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/services/commandService/commandService.py` & `nerualpha-5.0.0/src/nerualpha/smokes/assetsTest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
+from nerualpha.bridge import Bridge
 from nerualpha.IBridge import IBridge
+from nerualpha.session.ISession import ISession
+from nerualpha.providers.assets.assets import Assets
+from nerualpha.neru import Neru
 from nerualpha.request.requestParams import RequestParams
-from nerualpha.services.commandService.ICommandService import ICommandService
+from nerualpha.request.requestMethods import RequestMethods
 
 @dataclass
-class CommandService(ICommandService):
+class AssetsSmokeTests:
+    assets: Assets
+    session: ISession
     bridge: IBridge
-    def __init__(self,bridge):
-        self.bridge = bridge
+    healthChecksUrl: str = field(default = "https://hc-ping.com")
+    def __init__(self):
+        self.bridge = Bridge()
+        neru = Neru()
+        self.session = neru.createSession()
+        self.assets = Assets(self.session)
     
-    async def executeCommand(self,url,method,data = None,headers = None):
-        requestParams = RequestParams()
-        requestParams.url = url
-        requestParams.method = method
-        if data is not None:
-            requestParams.data = data
+    async def uploadAndGetRemoteFile(self,filePath: str,remoteDir: str,successPathname: str):
+        files = [filePath]
+        await self.assets.uploadFiles(files,remoteDir).execute()
+        file = await self.assets.getRemoteFile(remoteDir + "/" + filePath).execute()
+        if file is not None:
+            requestParams = RequestParams()
+            requestParams.method = RequestMethods.POST
+            requestParams.url = f'{self.healthChecksUrl}/{successPathname}'
+            await self.bridge.requestWithoutResponse(requestParams)
         
-        if headers is not None:
-            requestParams.headers = headers
-        
-        return await self.bridge.request(requestParams)
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/services/config/IConfig.py` & `nerualpha-5.0.0/src/nerualpha/services/config/IConfig.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     privateKey:str
     debug:bool
     appUrl:str
     assetUrl:str
     namespace:str
     logsSubmission:bool
     @abstractmethod
-    def getExecutionUrl(self,func,pathname = None,queryParams = None):
+    def getExecutionUrl(self,func: str,pathname: str = None,queryParams: Dict[str,str] = None):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/services/config/config.py` & `nerualpha-5.0.0/src/nerualpha/services/config/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     applicationId: str
     instanceServiceName: str
     bridge: IBridge
     instanceId: str = field(default = "debug")
     debug: bool = field(default = False)
     logsSubmission: bool = field(default = True)
     namespace: str = field(default = "neru")
-    def __init__(self,bridge):
+    def __init__(self,bridge: IBridge):
         self.bridge = bridge
         if self.bridge.getEnv("NAMESPACE") is not None:
             self.namespace = self.bridge.getEnv("NAMESPACE")
         
         self.instanceServiceName = self.bridge.getEnv("INSTANCE_SERVICE_NAME")
         self.applicationId = self.bridge.getEnv("APPLICATION_ID")
         if self.bridge.getEnv("INSTANCE_ID") is not None:
@@ -35,45 +35,45 @@
         self.appUrl = f'{self.bridge.getEnv("ENDPOINT_URL_SCHEME")}/{self.instanceServiceName}'
         debug = self.bridge.getEnv("DEBUG")
         if debug == "true":
             self.debug = True
         
         self.assetUrl = "http://openfaas.euw1.dev.nexmo.cloud/function/vonage-assets?get="
     
-    def getExecutionUrl(self,func,pathname = None,queryParams = None):
+    def getExecutionUrl(self,func: str,pathname: str = None,queryParams: Dict[str,str] = None):
         hostname = f'{func}.{self.namespace}'
         if self.debug:
             return self.constructDebugUrl(hostname,pathname,queryParams)
         
         return self.constructProdUrl(hostname,pathname,queryParams)
     
-    def constructDebugUrl(self,hostname,pathname,queryParams = None):
+    def constructDebugUrl(self,hostname: str,pathname: str,queryParams: Dict[str,str] = None):
         url = "http://localhost:3001"
         if pathname is not None:
             url += f'/{pathname}'
         
         url += f'?func={hostname}&async=false'
         if queryParams is not None:
             url += "&"
             url += self.queryObjectToString(queryParams)
         
         return url
     
-    def constructProdUrl(self,hostname,pathname,queryParams = None):
+    def constructProdUrl(self,hostname: str,pathname: str,queryParams: Dict[str,str] = None):
         url = f'http://{hostname}'
         if pathname is not None:
             url += f'/{pathname}'
         
         if queryParams is not None:
             url += "?"
             url += self.queryObjectToString(queryParams)
         
         return url
     
-    def queryObjectToString(self,queryObject):
+    def queryObjectToString(self,queryObject: Dict[str,str]):
         keys = self.bridge.getObjectKeys(queryObject)
         queryString = ""
         for i in range(0,keys.__len__()):
             key = keys[i]
             if queryObject[key] is not None:
                 encodedKey = self.bridge.encodeUriComponent(key)
                 value = self.bridge.encodeUriComponent(queryObject[key])
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/services/config/pathObject.py` & `nerualpha-5.0.0/src/nerualpha/services/config/pathObject.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/acl.py` & `nerualpha-5.0.0/src/nerualpha/providers/scheduler/contracts/schedulerPayload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.services.jwt.IAcl import IAcl
+from nerualpha.providers.scheduler.contracts.ISchedulePayload import ISchedulePayload
 
 @dataclass
-class Acl(IAcl):
-    paths: Dict[str,Dict[str,object]]
-    def __init__(self):
-        pass
+class SchedulerPayload(ISchedulePayload):
+    id: str
+    def __init__(self,id: str):
+        self.id = id
+    
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/createVonageTokenParams.py` & `nerualpha-5.0.0/src/nerualpha/services/jwt/createVonageTokenParams.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/jwt.py` & `nerualpha-5.0.0/src/nerualpha/services/jwt/jwt.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 @dataclass
 class JWT(IJWT):
     config: IConfig
     bridge: IBridge
     _token: str = field(default = None)
     ttl: int = field(default = 300)
-    def __init__(self,bridge,config):
+    def __init__(self,bridge: IBridge,config: IConfig):
         self.bridge = bridge
         self.config = config
     
     def getToken(self):
         try:
             if self._token is None or self.isExpired():
                 exp = self.bridge.getSystemTime() + self.ttl
@@ -34,23 +34,23 @@
     
     def isExpired(self):
         nowInSeconds = self.bridge.getSystemTime()
         twentySeconds = 20
         payload = self.bridge.jwtDecode(self._token)
         return payload["exp"] - twentySeconds <= nowInSeconds
     
-    def createNeruToken(self,exp):
+    def createNeruToken(self,exp: int):
         p = NeruJWTPayload()
         p.api_application_id = self.config.apiApplicationId
         p.api_account_id = self.config.apiAccountId
         p.exp = exp
         p.sub = self.config.instanceServiceName
         return self.bridge.jwtSign(p,self.config.privateKey,"RS256")
     
-    def createVonageToken(self,params):
+    def createVonageToken(self,params: ICreateVonageTokenParams):
         jwtPayload = VonageJWTPayload()
         jwtPayload.iat = self.bridge.getSystemTime()
         jwtPayload.exp = params.exp
         jwtPayload.application_id = self.config.apiApplicationId
         jwtPayload.jti = self.bridge.uuid()
         if params.aclPaths:
             jwtPayload.acl = Acl()
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/neruJWTPayload.py` & `nerualpha-5.0.0/src/nerualpha/services/jwt/neruJWTPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/services/jwt/vonageJWTPayload.py` & `nerualpha-5.0.0/src/nerualpha/services/jwt/vonageJWTPayload.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/ISession.py` & `nerualpha-5.0.0/src/nerualpha/session/ISession.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from nerualpha.providers.logger.ILogContext import ILogContext
 from nerualpha.services.commandService.ICommandService import ICommandService
 from nerualpha.services.config.IConfig import IConfig
 from nerualpha.services.jwt.IJwt import IJWT
 from nerualpha.session.IActionPayload import IActionPayload
 from nerualpha.session.IFilter import IFilter
 from nerualpha.session.wrappedCallback import WrappedCallback
-
+T = TypeVar('T')
+K = TypeVar('K')
 
 #interface
 class ISession(ABC):
     id:str
     commandService:ICommandService
     bridge:IBridge
     config:IConfig
@@ -22,21 +23,21 @@
     @abstractmethod
     def createUUID(self):
         pass
     @abstractmethod
     def getToken(self):
         pass
     @abstractmethod
-    def log(self,level,message,context):
+    def log(self,level: str,message: str,context: ILogContext):
         pass
     @abstractmethod
-    def wrapCallback(self,route,filters):
+    def wrapCallback(self,route: str,filters: List[IFilter]):
         pass
     @abstractmethod
     def constructCommandHeaders(self):
         pass
     @abstractmethod
     def constructRequestHeaders(self):
         pass
     @abstractmethod
-    def executeAction(self,actionPayload,method):
+    def executeAction(self,actionPayload: IActionPayload[T],method: str):
         pass
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/actionPayload.py` & `nerualpha-5.0.0/src/nerualpha/session/actionPayload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.session.IActionPayload import IActionPayload
 from nerualpha.session.IWrappedCallback import IWrappedCallback
-
+T = TypeVar('T')
 T = TypeVar("T")
 
 @dataclass
 class ActionPayload(IActionPayload,Generic[T]):
     payload: T
     action: str
     provider: str
     description: str = None
     successCallback: IWrappedCallback = None
     errorCallback: IWrappedCallback = None
-    def __init__(self,provider,action,payload,description = None):
+    def __init__(self,provider: str,action: str,payload: T,description: str = None):
         self.provider = provider
         self.action = action
         self.payload = payload
         if description is not None:
             self.description = description
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/command.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsVCardEvent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.session.IActionPayload import IActionPayload
-from nerualpha.session.ICommand import ICommand
-
-T = TypeVar("T")
+from nerualpha.webhookEvents.IUrlPayload import IUrlPayload
+from nerualpha.webhookEvents.mms.IMMSVCardEvent import IMMSVCardEvent
 
 @dataclass
-class Command(ICommand,Generic[T]):
-    actions: List[IActionPayload[T]]
-    header: Dict[str,str]
-    def __init__(self,headers,action):
-        self.header = headers
-        self.actions = [action]
-    
+class MMSVCardEvent(IMMSVCardEvent):
+    to: str
+    timestamp: str
+    message_uuid: str
+    message_type: str
+    from_: str
+    channel: str
+    vcard: IUrlPayload
+    def __init__(self):
+        pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/filter.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/viber/viberEvent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.session.IFilter import IFilter
+from nerualpha.webhookEvents.viber.IViberEvent import IViberEvent
 
 @dataclass
-class Filter(IFilter):
-    values: List[str]
-    op: str
-    path: str
-    def __init__(self,path,op,values):
-        self.path = path
-        self.op = op
-        self.values = values
-    
+class ViberEvent(IViberEvent):
+    to: str
+    timestamp: str
+    message_uuid: str
+    from_: str
+    channel: str
+    message_type: str
+    text: str
+    def __init__(self):
+        pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/neruSession.py` & `nerualpha-5.0.0/src/nerualpha/session/neruSession.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,57 +15,58 @@
 from nerualpha.services.jwt.IJwt import IJWT
 from nerualpha.session.command import Command
 from nerualpha.session.IActionPayload import IActionPayload
 from nerualpha.session.ICommand import ICommand
 from nerualpha.session.IFilter import IFilter
 from nerualpha.session.ISession import ISession
 from nerualpha.session.wrappedCallback import WrappedCallback
-
+T = TypeVar('T')
+K = TypeVar('K')
 @dataclass
 class NeruSession(ISession):
     eventEmitter: IEventEmitter
     commandService: ICommandService
     logger: ILogger
     bridge: IBridge
     jwt: IJWT
     config: IConfig
     id: str
-    def __init__(self,commandService,bridge,config,jwt,id):
+    def __init__(self,commandService: ICommandService,bridge: IBridge,config: IConfig,jwt: IJWT,id: str):
         self.commandService = commandService
         self.id = id
         self.bridge = bridge
         self.config = config
         self.jwt = jwt
         self.eventEmitter = EventEmitter(self)
         self.logger = Logger(self)
     
-    async def emitSessionCreatedEvent(self,ttl):
+    async def emitSessionCreatedEvent(self,ttl: int):
         await self.eventEmitter.emitSessionCreatedEvent(ttl)
     
     def createUUID(self):
         return self.bridge.uuid()
     
     def getToken(self):
         if self.config.debug:
             return None
         
         return self.jwt.getToken()
     
-    def log(self,level,message,context = None):
+    def log(self,level: str,message: str,context: ILogContext = None):
         if self.config.logsSubmission is False:
             self.bridge.log("Skipping sending logs as config.logsSubmission is set to false")
         
         elif self.bridge.getEnv("SKIP_LOGS_SUBMISSION") == "true":
             self.bridge.log("Skipping sending logs as SKIP_LOGS_SUBMISSION is set to true")
         
         else: 
             self.bridge.runBackgroundTask(self.logger.log(level,message,context))
         
     
-    def wrapCallback(self,route,filters):
+    def wrapCallback(self,route: str,filters: List[IFilter]):
         wrappedCallback = WrappedCallback()
         wrappedCallback.filters = filters
         wrappedCallback.id = self.createUUID()
         wrappedCallback.instanceServiceName = self.config.instanceServiceName
         wrappedCallback.sessionId = self.id
         wrappedCallback.instanceId = self.config.instanceId
         wrappedCallback.path = route
@@ -92,15 +93,15 @@
         headers["Content-Type"] = "application/json"
         token = self.getToken()
         if token is not None:
             headers["Authorization"] = f'Bearer {token}'
         
         return headers
     
-    async def executeAction(self,actionPayload,method):
+    async def executeAction(self,actionPayload: IActionPayload[T],method: str):
         try:
             commandHeaders = self.constructCommandHeaders()
             requestHeaders = self.constructRequestHeaders()
             payload = Command(commandHeaders,actionPayload)
             url = self.config.getExecutionUrl(actionPayload.provider)
             result = await self.commandService.executeCommand(url,method,payload,requestHeaders)
             context = LogContext(actionPayload.action,self.bridge.jsonStringify(actionPayload.payload),self.bridge.jsonStringify(result))
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/payloadWithCallback.py` & `nerualpha-5.0.0/src/nerualpha/session/payloadWithCallback.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from nerualpha.session.IPayloadWithCallback import IPayloadWithCallback
 from nerualpha.session.IWrappedCallback import IWrappedCallback
 
 @dataclass
 class PayloadWithCallback(IPayloadWithCallback):
     callback: IWrappedCallback
-    def __init__(self,callback):
+    def __init__(self,callback: IWrappedCallback):
         self.callback = callback
     
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/requestInterface.py` & `nerualpha-5.0.0/src/nerualpha/session/requestInterface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.session.ISession import ISession
 from nerualpha.session.IActionPayload import IActionPayload
 from nerualpha.request.requestMethods import RequestMethods
-
+T = TypeVar('T')
+K = TypeVar('K')
 T = TypeVar("T")
 K = TypeVar("K")
 
 @dataclass
 class RequestInterface(Generic[T,K]):
     method: str
     action: IActionPayload[T]
     session: ISession
-    def __init__(self,session,action,method = RequestMethods.POST):
+    def __init__(self,session: ISession,action: IActionPayload[T],method: str = RequestMethods.POST):
         self.session = session
         self.action = action
         self.method = method
     
-    def onSuccess(self,route):
+    def onSuccess(self,route: str):
         self.action.successCallback = self.session.wrapCallback(route,[])
         return self
     
-    def onError(self,route):
+    def onError(self,route: str):
         self.action.errorCallback = self.session.wrapCallback(route,[])
         return self
     
     async def execute(self):
         return await self.session.executeAction(self.action,self.method)
     
     def reprJSON(self):
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/requestInterfaceForCallbacks.py` & `nerualpha-5.0.0/src/nerualpha/session/requestInterfaceForCallbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.session.IPayloadWithCallback import IPayloadWithCallback
 from nerualpha.session.IActionPayload import IActionPayload
 from nerualpha.session.ISession import ISession
 from nerualpha.request.requestMethods import RequestMethods
-
+T = TypeVar('T')
 @dataclass
 class RequestInterfaceForCallbacks:
     method: str
     action: IActionPayload[IPayloadWithCallback]
     session: ISession
-    def __init__(self,session,action,method = RequestMethods.POST):
+    def __init__(self,session: ISession,action: IActionPayload[IPayloadWithCallback],method: str = RequestMethods.POST):
         self.session = session
         self.action = action
         self.method = method
     
     async def execute(self):
         await self.session.executeAction(self.action,self.method)
         return self.action.payload.callback.id
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/requestInterfaceWithParams.py` & `nerualpha-5.0.0/src/nerualpha/session/requestInterfaceWithParams.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.session.IRequestInterface import IRequestInterface
 from nerualpha.session.ISession import ISession
 from nerualpha.request.IRequestParams import IRequestParams
-
+T = TypeVar('T')
+K = TypeVar('K')
 T = TypeVar("T")
 K = TypeVar("K")
 
 @dataclass
 class RequestInterfaceWithParams(IRequestInterface,Generic[T,K]):
     requestParams: IRequestParams[T]
     session: ISession
-    def __init__(self,session,params):
+    def __init__(self,session: ISession,params: IRequestParams[T]):
         self.session = session
         self.requestParams = params
     
     async def execute(self):
         return await self.session.bridge.request(self.requestParams)
     
     def reprJSON(self):
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/session/wrappedCallback.py` & `nerualpha-5.0.0/src/nerualpha/session/wrappedCallback.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/smokes/messagesTest.py` & `nerualpha-5.0.0/src/nerualpha/smokes/messagesTest.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,48 +24,48 @@
     healthChecksUrl: str = field(default = "https://hc-ping.com")
     def __init__(self):
         self.bridge = Bridge()
         self.neru = Neru()
         self.session = self.neru.createSession()
         self.messages = Messages(self.session)
     
-    async def onMessage(self,callback,fromNumber,toNumber):
+    async def onMessage(self,callback: str,fromNumber: str,toNumber: str):
         fromContact = MessageContact()
         fromContact.type_ = "sms"
         fromContact.number = fromNumber
         toContact = MessageContact()
         toContact.type_ = "sms"
         toContact.number = toNumber
         await self.messages.onMessage(callback,fromContact,toContact).execute()
     
-    async def onEvent(self,callback,fromNumber,toNumber):
+    async def onEvent(self,callback: str,fromNumber: str,toNumber: str):
         clientContact = MessageContact()
         clientContact.type_ = "sms"
         clientContact.number = fromNumber
         applicationContact = MessageContact()
         applicationContact.type_ = "sms"
         applicationContact.number = toNumber
         await self.messages.onMessageEvents(callback,clientContact,applicationContact).execute()
     
-    async def sendMessage(self,fromNumber,toNumber,message):
+    async def sendMessage(self,fromNumber: str,toNumber: str,message: str):
         smsMessage = SMSMessage()
         smsMessage.from_ = fromNumber
         smsMessage.to = toNumber
         smsMessage.text = message
         await self.messages.send(smsMessage).execute()
     
-    async def checkIncomingMessageAndHitHealthEndpointIfSuccess(self,message,expectedMessage,successPathname):
+    async def checkIncomingMessageAndHitHealthEndpointIfSuccess(self,message: str,expectedMessage: str,successPathname: str):
         if message == expectedMessage:
             requestParams = RequestParams()
             requestParams.method = RequestMethods.POST
             requestParams.url = f'{self.healthChecksUrl}/{successPathname}'
             await self.bridge.requestWithoutResponse(requestParams)
         
     
-    async def checkIncomingEventAndHitHealthEndpointIfSuccess(self,sessionId,status,successPathname):
+    async def checkIncomingEventAndHitHealthEndpointIfSuccess(self,sessionId: str,status: str,successPathname: str):
         session = self.neru.getSessionById(sessionId)
         state = State(session)
         if status == "submitted":
             await state.incrby("submitted",1)
         
         if status == "delivered":
             await state.incrby("delivered",1)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/smokes/schedulerTest.py` & `nerualpha-5.0.0/src/nerualpha/smokes/schedulerTest.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,42 +27,42 @@
     healthChecksUrl: str = field(default = "https://hc-ping.com")
     def __init__(self):
         self.bridge = Bridge()
         self.neru = Neru()
         self.session = self.neru.createSession()
         self.scheduler = Scheduler(self.session)
     
-    async def scheduleOnce(self,callback):
+    async def scheduleOnce(self,callback: str):
         params = StartAtParams()
         params.startAt = self.bridge.isoDate()
         params.callback = callback
         params.payload = SchedulerTestPayload()
         await self.scheduler.startAt(params).execute()
     
-    async def scheduleRecurring(self,callback):
+    async def scheduleRecurring(self,callback: str):
         params = StartAtParams()
         params.startAt = self.bridge.isoDate()
         params.callback = callback
         params.payload = SchedulerTestPayload()
         params.interval = IntervalParams()
         params.interval.cron = "*/1 * * * *"
         params.interval.until = UntilParams()
         params.interval.until.maxInvocations = self.maxInvocations
         params.interval.until.date = self.bridge.toISOString(3 * 60)
         await self.scheduler.startAt(params).execute()
     
-    async def onScheduledOnce(self,payload,successPathname):
+    async def onScheduledOnce(self,payload: str,successPathname: str):
         if payload == "test payload":
             requestParams = RequestParams()
             requestParams.method = RequestMethods.POST
             requestParams.url = f'{self.healthChecksUrl}/{successPathname}'
             await self.bridge.requestWithoutResponse(requestParams)
         
     
-    async def onScheduledRecurring(self,sessionId,successPathname):
+    async def onScheduledRecurring(self,sessionId: str,successPathname: str):
         session = self.neru.getSessionById(sessionId)
         state = State(session)
         await state.incrby("count",1)
         count = await state.get("count")
         if count is self.maxInvocations:
             requestParams = RequestParams()
             requestParams.method = RequestMethods.POST
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/smokes/schedulerTestPayload.py` & `nerualpha-5.0.0/src/nerualpha/session/command.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
+from nerualpha.session.IActionPayload import IActionPayload
+from nerualpha.session.ICommand import ICommand
+T = TypeVar('T')
+T = TypeVar("T")
 
 @dataclass
-class SchedulerTestPayload:
-    text: str = field(default = "test payload")
-    def __init__(self):
-        pass
+class Command(ICommand,Generic[T]):
+    actions: List[IActionPayload[T]]
+    header: Dict[str,str]
+    def __init__(self,headers: Dict[str,str],action: IActionPayload[T]):
+        self.header = headers
+        self.actions = [action]
+    
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/smokes/stateTest.py` & `nerualpha-5.0.0/src/nerualpha/smokes/stateTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,27 @@
     healthChecksUrl: str = field(default = "https://hc-ping.com")
     def __init__(self):
         self.bridge = Bridge()
         self.neru = Neru()
         self.session = self.neru.createSession()
         self.state = State(self.session)
     
-    async def getset(self,successPathname):
+    async def getset(self,successPathname: str):
         key = "test-key"
         testData = "test-data"
         await self.state.set(key,testData)
         receivedData = await self.state.get(key)
         if receivedData == testData:
             requestParams = RequestParams()
             requestParams.method = RequestMethods.POST
             requestParams.url = f'{self.healthChecksUrl}/{successPathname}'
             await self.bridge.requestWithoutResponse(requestParams)
         
     
-    async def delete(self,successPathname):
+    async def delete(self,successPathname: str):
         key = "test-key"
         testData = "test-data"
         await self.state.set(key,testData)
         await self.state.delete(key)
         value = await self.state.get(key)
         if value is None:
             requestParams = RequestParams()
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/smokes/voiceTest.py` & `nerualpha-5.0.0/src/nerualpha/smokes/voiceTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.bridge = Bridge()
         self.neru = Neru()
         self.session = self.neru.createSession()
         self.voice = Voice(self.session)
         self.state = State(self.session)
         self.events = []
     
-    async def checkIncomingEventsAndHitHealthEndpointIfSuccessful(self,status,successPathname):
+    async def checkIncomingEventsAndHitHealthEndpointIfSuccessful(self,status: str,successPathname: str):
         await self.state.incrby(status,1)
         started = await self.state.get("started")
         ringing = await self.state.get("ringing")
         answered = await self.state.get("answered")
         completed = await self.state.get("completed")
         allEventsReceived = started and ringing and answered and completed
         if allEventsReceived:
@@ -44,24 +44,24 @@
             requestParams.method = "POST"
             requestParams.url = f'https://hc-ping.com/{successPathname}'
             await self.bridge.requestWithoutResponse(requestParams)
             self.events = []
         
         return
     
-    async def answer(self,event):
+    async def answer(self,event: IAcceptInboundCallEvent):
         conversation = await self.voice.createConversation()
         await conversation.acceptInboundCall(event).execute()
         await conversation.sayText({"text": "Hello from Vonage!"}).execute()
     
-    async def onInboundCall(self,callback,to):
+    async def onInboundCall(self,callback: str,to: str):
         vonageNumber = ChannelPhoneEndpoint(to)
         await self.voice.onInboundCall(callback,vonageNumber).execute()
     
-    async def call(self,fromNumber,toNumber,eventCallback):
+    async def call(self,fromNumber: str,toNumber: str,eventCallback: str):
         _fromNumber = ChannelPhoneEndpoint(fromNumber)
         _toNumber = ChannelPhoneEndpoint(toNumber)
         toNumbers = [_toNumber]
         nccoActions = [{"action": "talk","text": "Hello from Vonage! Listening for DTMF input..."},{"action": "input","type": ["dtmf"],"dtmf": {"maxDigits": 1,"submitOnHash": True,"timeOut": 10}}]
         response = await self.voice.vapiCreateCall(_fromNumber,toNumbers,nccoActions).execute()
         onEventParams = VapiEventParams()
         onEventParams.callback = eventCallback
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/baseEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/baseEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerAudioEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerAudioEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerFileEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerFileEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerImageEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerImageEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerTextEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerTextEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerUnsupportedEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerUnsupportedEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/messenger/messengerVideoEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/messenger/messengerVideoEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsAudioEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsAudioEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsImageEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsImageEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsVCardEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/mms/mmsVideoEvent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.webhookEvents.IUrlPayload import IUrlPayload
-from nerualpha.webhookEvents.mms.IMMSVCardEvent import IMMSVCardEvent
+from nerualpha.webhookEvents.mms.IMMSVideoEvent import IMMSVideoEvent
 
 @dataclass
-class MMSVCardEvent(IMMSVCardEvent):
+class MMSVideoEvent(IMMSVideoEvent):
     to: str
     timestamp: str
     message_uuid: str
     message_type: str
     from_: str
     channel: str
-    vcard: IUrlPayload
+    video: IUrlPayload
     def __init__(self):
         pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/mms/mmsVideoEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappVideoEvent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
 from nerualpha.webhookEvents.IUrlPayload import IUrlPayload
-from nerualpha.webhookEvents.mms.IMMSVideoEvent import IMMSVideoEvent
+from nerualpha.webhookEvents.whatsapp.IMessageEventContext import IMessageEventContext
+from nerualpha.webhookEvents.whatsapp.IProfileName import IProfileName
+from nerualpha.webhookEvents.whatsapp.IWhatsappVideoEvent import IWhatsappVideoEvent
 
 @dataclass
-class MMSVideoEvent(IMMSVideoEvent):
+class WhatsappVideoEvent(IWhatsappVideoEvent):
     to: str
     timestamp: str
     message_uuid: str
-    message_type: str
     from_: str
     channel: str
+    message_type: str
     video: IUrlPayload
+    profile: IProfileName = None
+    context: IMessageEventContext = None
+    provider_message: str = None
     def __init__(self):
         pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/smsEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsMetadata.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/smsMetadata.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/sms/smsUsage.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/sms/smsUsage.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/urlPayload.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/profileName.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.webhookEvents.IUrlPayload import IUrlPayload
+from nerualpha.webhookEvents.whatsapp.IProfileName import IProfileName
 
 @dataclass
-class UrlPayload(IUrlPayload):
-    url: str
+class ProfileName(IProfileName):
+    name: str
     def __init__(self):
         pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/viber/viberEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/messageEventContext.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.webhookEvents.viber.IViberEvent import IViberEvent
+from nerualpha.webhookEvents.whatsapp.IMessageEventContext import IMessageEventContext
 
 @dataclass
-class ViberEvent(IViberEvent):
-    to: str
-    timestamp: str
+class MessageEventContext(IMessageEventContext):
+    message_from: str
     message_uuid: str
-    from_: str
-    channel: str
-    message_type: str
-    text: str
     def __init__(self):
         pass
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/messageEventContext.py` & `nerualpha-5.0.0/src/nerualpha/providers/assets/contracts/linkPayload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.webhookEvents.whatsapp.IMessageEventContext import IMessageEventContext
 
 @dataclass
-class MessageEventContext(IMessageEventContext):
-    message_from: str
-    message_uuid: str
-    def __init__(self):
-        pass
+class LinkPayload:
+    duration: str
+    path: str
+    def __init__(self,path: str,duration: str):
+        self.path = path
+        self.duration = duration
+    
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/profileName.py` & `nerualpha-5.0.0/src/nerualpha/providers/meetings/contracts/updateRoomDetails.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.webhookEvents.whatsapp.IProfileName import IProfileName
 
 @dataclass
-class ProfileName(IProfileName):
-    name: str
-    def __init__(self):
-        pass
+class UpdateRoomDetails:
+    expire_after_use: bool
+    expires_at: str
+    def __init__(self,expires_at: str,expire_after_use: bool):
+        self.expires_at = expires_at
+        self.expire_after_use = expire_after_use
+    
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/replyObject.py` & `nerualpha-5.0.0/src/nerualpha/providers/voice/contracts/sayStopPayload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from dataclasses import dataclass, field, asdict
 from typing import Dict, List, Generic, TypeVar
 from abc import ABC, abstractmethod
 
-from nerualpha.webhookEvents.whatsapp.IReplyObject import IReplyObject
+from nerualpha.providers.voice.contracts.ISayStopPayload import ISayStopPayload
+from nerualpha.providers.voice.csEvents import CSEvents
+from nerualpha.providers.voice.contracts.ISayStopBody import ISayStopBody
+from nerualpha.providers.voice.contracts.sayStopBody import SayStopBody
 
 @dataclass
-class ReplyObject(IReplyObject):
-    title: str
-    id: str
-    description: str = None
-    def __init__(self):
-        pass
+class SayStopPayload(ISayStopPayload):
+    body: ISayStopBody
+    type_: str
+    to: str = None
+    def __init__(self,sayId: str,to: str = None):
+        self.type_ = CSEvents.AudioSayStop
+        self.body = SayStopBody(sayId)
+        if to is not None:
+            self.to = to
+        
+    
     def reprJSON(self):
         result = {}
         dict = asdict(self)
         keywordsMap = {"from_":"from","del_":"del","import_":"import","type_":"type"}
         for key in dict:
             val = getattr(self, key)
```

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappAudioEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappAudioEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappFileEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappFileEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappImageEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappImageEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappReplyEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappReplyEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappTextEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappTextEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/src/nerualpha/webhookEvents/whatsapp/whatsappUnsupportedEvent.py` & `nerualpha-5.0.0/src/nerualpha/webhookEvents/whatsapp/whatsappUnsupportedEvent.py`

 * *Files identical despite different names*

### Comparing `nerualpha-4.1.0rc5/PKG-INFO` & `nerualpha-5.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerualpha
-Version: 4.1.0rc5
+Version: 5.0.0
 Summary: neru-sdk for python developers
 License: MIT
 Author: Sergei Rastrigin
 Author-email: sergei.rastrigin@vonage.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

