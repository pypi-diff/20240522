# Comparing `tmp/ocpp-0.9.0.tar.gz` & `tmp/ocpp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocpp-0.9.0.tar", max compression
+gzip compressed data, was "ocpp-1.0.0.tar", max compression
```

## Comparing `ocpp-0.9.0.tar` & `ocpp-1.0.0.tar`

### file list

```diff
@@ -1,361 +1,226 @@
--rw-r--r--   0        0        0     1075 2021-05-29 12:40:10.211365 ocpp-0.9.0/LICENSE
--rw-r--r--   0        0        0     5803 2021-05-29 12:40:10.211365 ocpp-0.9.0/README.rst
--rw-r--r--   0        0        0        0 2021-05-29 12:40:10.338031 ocpp-0.9.0/ocpp/__init__.py
--rw-r--r--   0        0        0    11206 2021-06-29 19:28:41.218264 ocpp-0.9.0/ocpp/charge_point.py
--rw-r--r--   0        0        0     3168 2021-07-23 11:26:56.054943 ocpp-0.9.0/ocpp/exceptions.py
--rw-r--r--   0        0        0    15020 2021-09-02 10:31:37.936056 ocpp-0.9.0/ocpp/messages.py
--rw-r--r--   0        0        0     4084 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/routing.py
--rw-r--r--   0        0        0      186 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/__init__.py
--rw-r--r--   0        0        0     6162 2021-09-02 10:31:37.936056 ocpp-0.9.0/ocpp/v16/call.py
--rw-r--r--   0        0        0     4773 2021-09-02 10:31:37.936056 ocpp-0.9.0/ocpp/v16/call_result.py
--rw-r--r--   0        0        0    21190 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/enums.py
--rw-r--r--   0        0        0      306 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/Authorize.json
--rw-r--r--   0        0        0     1062 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/AuthorizeResponse.json
--rw-r--r--   0        0        0     1139 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/BootNotification.json
--rw-r--r--   0        0        0      655 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/BootNotificationResponse.json
--rw-r--r--   0        0        0      302 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/CancelReservation.json
--rw-r--r--   0        0        0      423 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/CancelReservationResponse.json
--rw-r--r--   0        0        0      352 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/CertificateSigned.json
--rw-r--r--   0        0        0      505 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/CertificateSignedResponse.json
--rw-r--r--   0        0        0      512 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ChangeAvailability.json
--rw-r--r--   0        0        0      453 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ChangeAvailabilityResponse.json
--rw-r--r--   0        0        0      418 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ChangeConfiguration.json
--rw-r--r--   0        0        0      491 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ChangeConfigurationResponse.json
--rw-r--r--   0        0        0      174 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ClearCache.json
--rw-r--r--   0        0        0      416 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ClearCacheResponse.json
--rw-r--r--   0        0        0      637 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ClearChargingProfile.json
--rw-r--r--   0        0        0      425 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ClearChargingProfileResponse.json
--rw-r--r--   0        0        0      466 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/DataTransfer.json
--rw-r--r--   0        0        0      547 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/DataTransferResponse.json
--rw-r--r--   0        0        0     1156 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/DeleteCertificate.json
--rw-r--r--   0        0        0      523 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/DeleteCertificateResponse.json
--rw-r--r--   0        0        0      491 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/DiagnosticsStatusNotification.json
--rw-r--r--   0        0        0      194 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/DiagnosticsStatusNotificationResponse.json
--rw-r--r--   0        0        0      760 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/ExtendedTriggerMessage.json
--rw-r--r--   0        0        0      530 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json
--rw-r--r--   0        0        0      591 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/FirmwareStatusNotification.json
--rw-r--r--   0        0        0      191 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/FirmwareStatusNotificationResponse.json
--rw-r--r--   0        0        0      539 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetCompositeSchedule.json
--rw-r--r--   0        0        0     2139 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetCompositeScheduleResponse.json
--rw-r--r--   0        0        0      344 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetConfiguration.json
--rw-r--r--   0        0        0     1066 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetConfigurationResponse.json
--rw-r--r--   0        0        0      642 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetDiagnostics.json
--rw-r--r--   0        0        0      275 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetDiagnosticsResponse.json
--rw-r--r--   0        0        0      552 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/GetInstalledCertificateIds.json
--rw-r--r--   0        0        0     1566 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json
--rw-r--r--   0        0        0      183 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetLocalListVersion.json
--rw-r--r--   0        0        0      301 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetLocalListVersionResponse.json
--rw-r--r--   0        0        0     1184 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/GetLog.json
--rw-r--r--   0        0        0      566 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/GetLogResponse.json
--rw-r--r--   0        0        0      173 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/Heartbeat.json
--rw-r--r--   0        0        0      325 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/HeartbeatResponse.json
--rw-r--r--   0        0        0      639 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/InstallCertificate.json
--rw-r--r--   0        0        0      526 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/InstallCertificateResponse.json
--rw-r--r--   0        0        0      667 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/LogStatusNotification.json
--rw-r--r--   0        0        0      173 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/LogStatusNotificationResponse.json
--rw-r--r--   0        0        0     6758 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/MeterValues.json
--rw-r--r--   0        0        0      176 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/MeterValuesResponse.json
--rw-r--r--   0        0        0     4383 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/RemoteStartTransaction.json
--rw-r--r--   0        0        0      428 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/RemoteStartTransactionResponse.json
--rw-r--r--   0        0        0      306 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/RemoteStopTransaction.json
--rw-r--r--   0        0        0      427 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/RemoteStopTransactionResponse.json
--rw-r--r--   0        0        0      704 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ReserveNow.json
--rw-r--r--   0        0        0      502 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ReserveNowResponse.json
--rw-r--r--   0        0        0      398 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/Reset.json
--rw-r--r--   0        0        0      411 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ResetResponse.json
--rw-r--r--   0        0        0      464 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SecurityEventNotification.json
--rw-r--r--   0        0        0      177 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SecurityEventNotificationResponse.json
--rw-r--r--   0        0        0     2146 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/SendLocalList.json
--rw-r--r--   0        0        0      484 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/SendLocalListResponse.json
--rw-r--r--   0        0        0     4310 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/SetChargingProfile.json
--rw-r--r--   0        0        0      456 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/SetChargingProfileResponse.json
--rw-r--r--   0        0        0      287 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignCertificate.json
--rw-r--r--   0        0        0      483 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignCertificateResponse.json
--rw-r--r--   0        0        0      876 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignedFirmwareStatusNotification.json
--rw-r--r--   0        0        0      184 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignedFirmwareStatusNotificationResponse.json
--rw-r--r--   0        0        0     1212 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignedUpdateFirmware.json
--rw-r--r--   0        0        0      590 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json
--rw-r--r--   0        0        0      676 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StartTransaction.json
--rw-r--r--   0        0        0     1162 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StartTransactionResponse.json
--rw-r--r--   0        0        0     1805 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StatusNotification.json
--rw-r--r--   0        0        0      183 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StatusNotificationResponse.json
--rw-r--r--   0        0        0     7313 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StopTransaction.json
--rw-r--r--   0        0        0     1023 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StopTransactionResponse.json
--rw-r--r--   0        0        0      678 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/TriggerMessage.json
--rw-r--r--   0        0        0      454 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/TriggerMessageResponse.json
--rw-r--r--   0        0        0      296 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/UnlockConnector.json
--rw-r--r--   0        0        0      457 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/UnlockConnectorResponse.json
--rw-r--r--   0        0        0      572 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/UpdateFirmware.json
--rw-r--r--   0        0        0      179 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/UpdateFirmwareResponse.json
--rw-r--r--   0        0        0      186 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/__init__.py
--rw-r--r--   0        0        0     7491 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/call.py
--rw-r--r--   0        0        0     4907 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/call_result.py
--rw-r--r--   0        0        0     2971 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/AuthorizeRequest_v1p0.json
--rw-r--r--   0        0        0     3495 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/AuthorizeResponse_v1p0.json
--rw-r--r--   0        0        0     1771 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/BootNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      560 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/BootNotificationResponse_v1p0.json
--rw-r--r--   0        0        0      275 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CancelReservationRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CancelReservationResponse_v1p0.json
--rw-r--r--   0        0        0      580 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CertificateSignedRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CertificateSignedResponse_v1p0.json
--rw-r--r--   0        0        0      456 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ChangeAvailabilityRequest_v1p0.json
--rw-r--r--   0        0        0      387 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ChangeAvailabilityResponse_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearCacheRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearCacheResponse_v1p0.json
--rw-r--r--   0        0        0     1029 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearChargingProfileRequest_v1p0.json
--rw-r--r--   0        0        0      364 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearChargingProfileResponse_v1p0.json
--rw-r--r--   0        0        0      253 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearDisplayMessageRequest_v1p0.json
--rw-r--r--   0        0        0      364 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearDisplayMessageResponse_v1p0.json
--rw-r--r--   0        0        0      361 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearVariableMonitoringRequest_v1p0.json
--rw-r--r--   0        0        0     1055 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearVariableMonitoringResponse_v1p0.json
--rw-r--r--   0        0        0      464 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearedChargingLimitRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearedChargingLimitResponse_v1p0.json
--rw-r--r--   0        0        0      368 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CostUpdatedRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CostUpdatedResponse_v1p0.json
--rw-r--r--   0        0        0     2862 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CustomerInformationRequest_v1p0.json
--rw-r--r--   0        0        0      385 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CustomerInformationResponse_v1p0.json
--rw-r--r--   0        0        0      382 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/DataTransferRequest_v1p0.json
--rw-r--r--   0        0        0      439 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/DataTransferResponse_v1p0.json
--rw-r--r--   0        0        0     1224 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/DeleteCertificateRequest_v1p0.json
--rw-r--r--   0        0        0      384 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/DeleteCertificateResponse_v1p0.json
--rw-r--r--   0        0        0      893 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/FirmwareStatusNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/FirmwareStatusNotificationResponse_v1p0.json
--rw-r--r--   0        0        0      406 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/Get15118EVCertificateRequest_v1p0.json
--rw-r--r--   0        0        0     1465 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/Get15118EVCertificateResponse_v1p0.json
--rw-r--r--   0        0        0      492 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetBaseReportRequest_v1p0.json
--rw-r--r--   0        0        0      390 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetBaseReportResponse_v1p0.json
--rw-r--r--   0        0        0     1300 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetCertificateStatusRequest_v1p0.json
--rw-r--r--   0        0        0      444 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetCertificateStatusResponse_v1p0.json
--rw-r--r--   0        0        0     1744 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetChargingProfilesRequest_v1p0.json
--rw-r--r--   0        0        0      367 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetChargingProfilesResponse_v1p0.json
--rw-r--r--   0        0        0      480 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetCompositeScheduleRequest_v1p0.json
--rw-r--r--   0        0        0     2510 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetCompositeScheduleResponse_v1p0.json
--rw-r--r--   0        0        0      796 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetDisplayMessagesRequest_v1p0.json
--rw-r--r--   0        0        0      364 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetDisplayMessagesResponse_v1p0.json
--rw-r--r--   0        0        0      521 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetInstalledCertificateIdsRequest_v1p0.json
--rw-r--r--   0        0        0     1598 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetInstalledCertificateIdsResponse_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetLocalListVersionRequest_v1p0.json
--rw-r--r--   0        0        0      275 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetLocalListVersionResponse_v1p0.json
--rw-r--r--   0        0        0     1264 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetLogRequest_v1p0.json
--rw-r--r--   0        0        0      470 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetLogResponse_v1p0.json
--rw-r--r--   0        0        0     2467 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetMonitoringReportRequest_v1p0.json
--rw-r--r--   0        0        0      390 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetMonitoringReportResponse_v1p0.json
--rw-r--r--   0        0        0     2454 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetReportRequest_v1p0.json
--rw-r--r--   0        0        0      390 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetReportResponse_v1p0.json
--rw-r--r--   0        0        0      254 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetTransactionStatusRequest_v1p0.json
--rw-r--r--   0        0        0      339 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetTransactionStatusResponse_v1p0.json
--rw-r--r--   0        0        0     2322 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetVariablesRequest_v1p0.json
--rw-r--r--   0        0        0     2830 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetVariablesResponse_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/HeartbeatRequest_v1p0.json
--rw-r--r--   0        0        0      300 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/HeartbeatResponse_v1p0.json
--rw-r--r--   0        0        0      616 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/InstallCertificateRequest_v1p0.json
--rw-r--r--   0        0        0      525 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/InstallCertificateResponse_v1p0.json
--rw-r--r--   0        0        0      566 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/LogStatusNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/LogStatusNotificationResponse_v1p0.json
--rw-r--r--   0        0        0     5109 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/MeterValuesRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/MeterValuesResponse_v1p0.json
--rw-r--r--   0        0        0     4477 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyCentralChargingNeedsRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyCentralChargingNeedsResponse_v1p0.json
--rw-r--r--   0        0        0     2690 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyChargingLimitRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyChargingLimitResponse_v1p0.json
--rw-r--r--   0        0        0      560 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyCustomerInformationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyCustomerInformationResponse_v1p0.json
--rw-r--r--   0        0        0     3393 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyDisplayMessagesRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyDisplayMessagesResponse_v1p0.json
--rw-r--r--   0        0        0     2943 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingNeedsRequest_v1p0.json
--rw-r--r--   0        0        0      388 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingNeedsResponse_v1p0.json
--rw-r--r--   0        0        0     1978 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingScheduleRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingScheduleResponse_v1p0.json
--rw-r--r--   0        0        0     4157 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEventRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEventResponse_v1p0.json
--rw-r--r--   0        0        0     3429 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyMonitoringReportRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyMonitoringReportResponse_v1p0.json
--rw-r--r--   0        0        0     4752 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyReportRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyReportResponse_v1p0.json
--rw-r--r--   0        0        0      432 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/PublishFirmwareRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/PublishFirmwareResponse_v1p0.json
--rw-r--r--   0        0        0      637 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/PublishFirmwareStatusNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/PublishFirmwareStatusNotificationResponse_v1p0.json
--rw-r--r--   0        0        0      614 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/Renegotiate15118ScheduleRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/Renegotiate15118ScheduleResponse_v1p0.json
--rw-r--r--   0        0        0     4309 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReportChargingProfilesRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReportChargingProfilesResponse_v1p0.json
--rw-r--r--   0        0        0     5216 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/RequestStartTransactionRequest_v1p0.json
--rw-r--r--   0        0        0      445 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/RequestStartTransactionResponse_v1p0.json
--rw-r--r--   0        0        0      298 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/RequestStopTransactionRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/RequestStopTransactionResponse_v1p0.json
--rw-r--r--   0        0        0      476 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReservationStatusUpdateRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReservationStatusUpdateResponse_v1p0.json
--rw-r--r--   0        0        0     3277 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReserveNowRequest_v1p0.json
--rw-r--r--   0        0        0      430 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReserveNowResponse_v1p0.json
--rw-r--r--   0        0        0      360 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ResetRequest_v1p0.json
--rw-r--r--   0        0        0      387 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/ResetResponse_v1p0.json
--rw-r--r--   0        0        0     1049 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SecurityEventNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SecurityEventNotificationResponse_v1p0.json
--rw-r--r--   0        0        0     4782 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SendLocalListRequest_v1p0.json
--rw-r--r--   0        0        0      391 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SendLocalListResponse_v1p0.json
--rw-r--r--   0        0        0     3778 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetChargingProfileRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetChargingProfileResponse_v1p0.json
--rw-r--r--   0        0        0     3147 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetDisplayMessageRequest_v1p0.json
--rw-r--r--   0        0        0      497 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetDisplayMessageResponse_v1p0.json
--rw-r--r--   0        0        0      399 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetMonitoringBaseRequest_v1p0.json
--rw-r--r--   0        0        0      390 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetMonitoringBaseResponse_v1p0.json
--rw-r--r--   0        0        0      269 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetMonitoringLevelRequest_v1p0.json
--rw-r--r--   0        0        0      369 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetMonitoringLevelResponse_v1p0.json
--rw-r--r--   0        0        0     4030 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetNetworkProfileRequest_v1p0.json
--rw-r--r--   0        0        0      384 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetNetworkProfileResponse_v1p0.json
--rw-r--r--   0        0        0     2646 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetVariableMonitoringRequest_v1p0.json
--rw-r--r--   0        0        0     2938 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetVariableMonitoringResponse_v1p0.json
--rw-r--r--   0        0        0     2448 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetVariablesRequest_v1p0.json
--rw-r--r--   0        0        0     2806 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetVariablesResponse_v1p0.json
--rw-r--r--   0        0        0      468 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SignCertificateRequest_v1p0.json
--rw-r--r--   0        0        0      365 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SignCertificateResponse_v1p0.json
--rw-r--r--   0        0        0      689 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/StatusNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/StatusNotificationResponse_v1p0.json
--rw-r--r--   0        0        0     9743 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/TransactionEventRequest_v1p0.json
--rw-r--r--   0        0        0     3072 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/TransactionEventResponse_v1p0.json
--rw-r--r--   0        0        0     1125 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/TriggerMessageRequest_v1p0.json
--rw-r--r--   0        0        0      392 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/TriggerMessageResponse_v1p0.json
--rw-r--r--   0        0        0      336 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UnlockConnectorRequest_v1p0.json
--rw-r--r--   0        0        0      369 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UnlockConnectorResponse_v1p0.json
--rw-r--r--   0        0        0      290 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UnpublishFirmwareRequest_v1p0.json
--rw-r--r--   0        0        0      398 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UnpublishFirmwareResponse_v1p0.json
--rw-r--r--   0        0        0      406 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/Update15118EVCertificateRequest_v1p0.json
--rw-r--r--   0        0        0      443 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/Update15118EVCertificateResponse_v1p0.json
--rw-r--r--   0        0        0     1219 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UpdateFirmwareRequest_v1p0.json
--rw-r--r--   0        0        0      394 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UpdateFirmwareResponse_v1p0.json
--rw-r--r--   0        0        0      189 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/__init__.py
--rw-r--r--   0        0        0     7665 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/call.py
--rw-r--r--   0        0        0     6013 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/call_result.py
--rw-r--r--   0        0        0    32670 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/enums.py
--rwxr-xr-x   0        0        0     4203 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/AuthorizeRequest.json
--rwxr-xr-x   0        0        0     7208 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/AuthorizeResponse.json
--rwxr-xr-x   0        0        0     3161 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/BootNotificationRequest.json
--rwxr-xr-x   0        0        0     2270 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/BootNotificationResponse.json
--rwxr-xr-x   0        0        0      775 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CancelReservationRequest.json
--rwxr-xr-x   0        0        0     1758 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CancelReservationResponse.json
--rwxr-xr-x   0        0        0     1914 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CertificateSignedRequest.json
--rwxr-xr-x   0        0        0     1752 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CertificateSignedResponse.json
--rwxr-xr-x   0        0        0     1811 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ChangeAvailabilityRequest.json
--rwxr-xr-x   0        0        0     1783 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ChangeAvailabilityResponse.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearCacheRequest.json
--rwxr-xr-x   0        0        0     1735 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearCacheResponse.json
--rwxr-xr-x   0        0        0     2574 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearChargingProfileRequest.json
--rwxr-xr-x   0        0        0     1752 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearChargingProfileResponse.json
--rwxr-xr-x   0        0        0      787 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearDisplayMessageRequest.json
--rwxr-xr-x   0        0        0     1735 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearDisplayMessageResponse.json
--rwxr-xr-x   0        0        0      865 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearVariableMonitoringRequest.json
--rwxr-xr-x   0        0        0     2327 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearVariableMonitoringResponse.json
--rwxr-xr-x   0        0        0     1087 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearedChargingLimitRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearedChargingLimitResponse.json
--rwxr-xr-x   0        0        0     1121 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CostUpdatedRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CostUpdatedResponse.json
--rwxr-xr-x   0        0        0     4659 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CustomerInformationRequest.json
--rwxr-xr-x   0        0        0     1740 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CustomerInformationResponse.json
--rwxr-xr-x   0        0        0     1101 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/DataTransferRequest.json
--rwxr-xr-x   0        0        0     1869 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/DataTransferResponse.json
--rwxr-xr-x   0        0        0     1808 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/DeleteCertificateRequest.json
--rwxr-xr-x   0        0        0     1747 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/DeleteCertificateResponse.json
--rwxr-xr-x   0        0        0     1539 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json
--rwxr-xr-x   0        0        0     1424 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/Get15118EVCertificateRequest.json
--rwxr-xr-x   0        0        0     1914 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/Get15118EVCertificateResponse.json
--rwxr-xr-x   0        0        0     1105 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetBaseReportRequest.json
--rwxr-xr-x   0        0        0     1794 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetBaseReportResponse.json
--rwxr-xr-x   0        0        0     1957 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetCertificateStatusRequest.json
--rwxr-xr-x   0        0        0     2089 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetCertificateStatusResponse.json
--rwxr-xr-x   0        0        0     3622 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetChargingProfilesRequest.json
--rwxr-xr-x   0        0        0     1859 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetChargingProfilesResponse.json
--rwxr-xr-x   0        0        0     1329 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetCompositeScheduleRequest.json
--rwxr-xr-x   0        0        0     5095 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetCompositeScheduleResponse.json
--rwxr-xr-x   0        0        0     1874 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetDisplayMessagesRequest.json
--rwxr-xr-x   0        0        0     1841 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetDisplayMessagesResponse.json
--rwxr-xr-x   0        0        0     1204 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json
--rwxr-xr-x   0        0        0     3997 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetLocalListVersionRequest.json
--rwxr-xr-x   0        0        0      840 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetLocalListVersionResponse.json
--rwxr-xr-x   0        0        0     2802 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetLogRequest.json
--rwxr-xr-x   0        0        0     1954 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetLogResponse.json
--rwxr-xr-x   0        0        0     4175 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetMonitoringReportRequest.json
--rwxr-xr-x   0        0        0     1800 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetMonitoringReportResponse.json
--rwxr-xr-x   0        0        0     4143 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetReportRequest.json
--rwxr-xr-x   0        0        0     1800 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetReportResponse.json
--rwxr-xr-x   0        0        0      784 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetTransactionStatusRequest.json
--rwxr-xr-x   0        0        0      910 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetTransactionStatusResponse.json
--rwxr-xr-x   0        0        0     3931 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetVariablesRequest.json
--rwxr-xr-x   0        0        0     5581 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetVariablesResponse.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/HeartbeatRequest.json
--rwxr-xr-x   0        0        0      802 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/HeartbeatResponse.json
--rwxr-xr-x   0        0        0     1226 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/InstallCertificateRequest.json
--rwxr-xr-x   0        0        0     1751 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/InstallCertificateResponse.json
--rwxr-xr-x   0        0        0     1361 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/LogStatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/LogStatusNotificationResponse.json
--rwxr-xr-x   0        0        0     7709 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/MeterValuesRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/MeterValuesResponse.json
--rwxr-xr-x   0        0        0    11333 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyChargingLimitRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyChargingLimitResponse.json
--rwxr-xr-x   0        0        0     1542 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyCustomerInformationRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyCustomerInformationResponse.json
--rwxr-xr-x   0        0        0     6512 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json
--rwxr-xr-x   0        0        0     5943 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json
--rwxr-xr-x   0        0        0     1870 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json
--rwxr-xr-x   0        0        0    10370 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json
--rwxr-xr-x   0        0        0     1780 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json
--rwxr-xr-x   0        0        0     6614 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEventRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEventResponse.json
--rwxr-xr-x   0        0        0     7005 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyMonitoringReportRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyMonitoringReportResponse.json
--rwxr-xr-x   0        0        0     8608 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyReportRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyReportResponse.json
--rwxr-xr-x   0        0        0     1668 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareRequest.json
--rwxr-xr-x   0        0        0     1691 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareResponse.json
--rwxr-xr-x   0        0        0     1631 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json
--rwxr-xr-x   0        0        0    14700 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReportChargingProfilesRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReportChargingProfilesResponse.json
--rwxr-xr-x   0        0        0    15964 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/RequestStartTransactionRequest.json
--rwxr-xr-x   0        0        0     2080 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/RequestStartTransactionResponse.json
--rwxr-xr-x   0        0        0      844 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/RequestStopTransactionRequest.json
--rwxr-xr-x   0        0        0     1760 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/RequestStopTransactionResponse.json
--rwxr-xr-x   0        0        0     1133 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReservationStatusUpdateRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReservationStatusUpdateResponse.json
--rwxr-xr-x   0        0        0     3649 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReserveNowRequest.json
--rwxr-xr-x   0        0        0     1758 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReserveNowResponse.json
--rwxr-xr-x   0        0        0     1144 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ResetRequest.json
--rwxr-xr-x   0        0        0     1730 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ResetResponse.json
--rwxr-xr-x   0        0        0     1120 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/SecurityEventNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/SecurityEventNotificationResponse.json
--rwxr-xr-x   0        0        0     7733 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SendLocalListRequest.json
--rwxr-xr-x   0        0        0     1810 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SendLocalListResponse.json
--rwxr-xr-x   0        0        0    13730 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetChargingProfileRequest.json
--rwxr-xr-x   0        0        0     1913 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetChargingProfileResponse.json
--rwxr-xr-x   0        0        0     5989 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetDisplayMessageRequest.json
--rwxr-xr-x   0        0        0     1848 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetDisplayMessageResponse.json
--rwxr-xr-x   0        0        0     1005 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringBaseRequest.json
--rwxr-xr-x   0        0        0     1789 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringBaseResponse.json
--rwxr-xr-x   0        0        0     2087 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringLevelRequest.json
--rwxr-xr-x   0        0        0     1718 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringLevelResponse.json
--rwxr-xr-x   0        0        0     7613 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetNetworkProfileRequest.json
--rwxr-xr-x   0        0        0     1710 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetNetworkProfileResponse.json
--rwxr-xr-x   0        0        0     5959 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetVariableMonitoringRequest.json
--rwxr-xr-x   0        0        0     6923 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetVariableMonitoringResponse.json
--rwxr-xr-x   0        0        0     4272 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetVariablesRequest.json
--rwxr-xr-x   0        0        0     5035 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetVariablesResponse.json
--rwxr-xr-x   0        0        0     1481 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SignCertificateRequest.json
--rwxr-xr-x   0        0        0     1699 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SignCertificateResponse.json
--rwxr-xr-x   0        0        0     1570 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/StatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/StatusNotificationResponse.json
--rwxr-xr-x   0        0        0    14824 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/TransactionEventRequest.json
--rwxr-xr-x   0        0        0     7606 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/TransactionEventResponse.json
--rwxr-xr-x   0        0        0     1996 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/TriggerMessageRequest.json
--rwxr-xr-x   0        0        0     1772 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/TriggerMessageResponse.json
--rwxr-xr-x   0        0        0      970 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UnlockConnectorRequest.json
--rwxr-xr-x   0        0        0     1776 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UnlockConnectorResponse.json
--rwxr-xr-x   0        0        0      837 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UnpublishFirmwareRequest.json
--rwxr-xr-x   0        0        0     1059 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UnpublishFirmwareResponse.json
--rwxr-xr-x   0        0        0     2765 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UpdateFirmwareRequest.json
--rwxr-xr-x   0        0        0     1824 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UpdateFirmwareResponse.json
--rw-r--r--   0        0        0     1585 2021-09-02 10:41:18.516842 ocpp-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     7017 2021-09-02 10:42:47.379849 ocpp-0.9.0/setup.py
--rw-r--r--   0        0        0     6758 2021-09-02 10:42:47.380375 ocpp-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-09-27 14:02:09.595736 ocpp-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6872 2024-05-14 14:34:08.955627 ocpp-1.0.0/README.rst
+-rw-r--r--   0        0        0        0 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/__init__.py
+-rw-r--r--   0        0        0    16259 2024-05-07 10:02:50.787007 ocpp-1.0.0/ocpp/charge_point.py
+-rw-r--r--   0        0        0     4451 2024-02-05 14:06:46.101172 ocpp-1.0.0/ocpp/exceptions.py
+-rw-r--r--   0        0        0      221 2024-05-07 10:02:50.787007 ocpp-1.0.0/ocpp/experimental/v21/README.rst
+-rw-r--r--   0        0        0    14821 2024-02-05 14:06:46.101172 ocpp-1.0.0/ocpp/messages.py
+-rw-r--r--   0        0        0     4106 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/routing.py
+-rw-r--r--   0        0        0      186 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/__init__.py
+-rw-r--r--   0        0        0    20548 2024-02-05 14:06:46.101172 ocpp-1.0.0/ocpp/v16/call.py
+-rw-r--r--   0        0        0    19232 2024-02-05 14:06:46.101172 ocpp-1.0.0/ocpp/v16/call_result.py
+-rw-r--r--   0        0        0     3968 2024-02-05 14:06:46.101172 ocpp-1.0.0/ocpp/v16/datatypes.py
+-rw-r--r--   0        0        0    23663 2024-05-07 10:02:50.787007 ocpp-1.0.0/ocpp/v16/enums.py
+-rw-r--r--   0        0        0      306 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/Authorize.json
+-rw-r--r--   0        0        0     1062 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/AuthorizeResponse.json
+-rw-r--r--   0        0        0     1139 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/BootNotification.json
+-rw-r--r--   0        0        0      655 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/BootNotificationResponse.json
+-rw-r--r--   0        0        0      302 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/CancelReservation.json
+-rw-r--r--   0        0        0      423 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/CancelReservationResponse.json
+-rw-r--r--   0        0        0      352 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/CertificateSigned.json
+-rw-r--r--   0        0        0      505 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/CertificateSignedResponse.json
+-rw-r--r--   0        0        0      512 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ChangeAvailability.json
+-rw-r--r--   0        0        0      453 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ChangeAvailabilityResponse.json
+-rw-r--r--   0        0        0      418 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ChangeConfiguration.json
+-rw-r--r--   0        0        0      491 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ChangeConfigurationResponse.json
+-rw-r--r--   0        0        0      174 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ClearCache.json
+-rw-r--r--   0        0        0      416 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ClearCacheResponse.json
+-rw-r--r--   0        0        0      637 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ClearChargingProfile.json
+-rw-r--r--   0        0        0      425 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ClearChargingProfileResponse.json
+-rw-r--r--   0        0        0      466 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/DataTransfer.json
+-rw-r--r--   0        0        0      547 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/DataTransferResponse.json
+-rw-r--r--   0        0        0     1156 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/DeleteCertificate.json
+-rw-r--r--   0        0        0      523 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/DeleteCertificateResponse.json
+-rw-r--r--   0        0        0      491 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/DiagnosticsStatusNotification.json
+-rw-r--r--   0        0        0      194 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/DiagnosticsStatusNotificationResponse.json
+-rw-r--r--   0        0        0      760 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ExtendedTriggerMessage.json
+-rw-r--r--   0        0        0      530 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json
+-rw-r--r--   0        0        0      591 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/FirmwareStatusNotification.json
+-rw-r--r--   0        0        0      191 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/FirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0      539 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetCompositeSchedule.json
+-rw-r--r--   0        0        0     2139 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetCompositeScheduleResponse.json
+-rw-r--r--   0        0        0      344 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetConfiguration.json
+-rw-r--r--   0        0        0     1066 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetConfigurationResponse.json
+-rw-r--r--   0        0        0      642 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetDiagnostics.json
+-rw-r--r--   0        0        0      275 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetDiagnosticsResponse.json
+-rw-r--r--   0        0        0      552 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetInstalledCertificateIds.json
+-rw-r--r--   0        0        0     1566 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json
+-rw-r--r--   0        0        0      183 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetLocalListVersion.json
+-rw-r--r--   0        0        0      301 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetLocalListVersionResponse.json
+-rw-r--r--   0        0        0     1184 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetLog.json
+-rw-r--r--   0        0        0      566 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/GetLogResponse.json
+-rw-r--r--   0        0        0      173 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/Heartbeat.json
+-rw-r--r--   0        0        0      325 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/HeartbeatResponse.json
+-rw-r--r--   0        0        0      639 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/InstallCertificate.json
+-rw-r--r--   0        0        0      526 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/InstallCertificateResponse.json
+-rw-r--r--   0        0        0      667 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/LogStatusNotification.json
+-rw-r--r--   0        0        0      173 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/LogStatusNotificationResponse.json
+-rw-r--r--   0        0        0     6758 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/MeterValues.json
+-rw-r--r--   0        0        0      176 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/MeterValuesResponse.json
+-rw-r--r--   0        0        0     4383 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/RemoteStartTransaction.json
+-rw-r--r--   0        0        0      428 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/RemoteStartTransactionResponse.json
+-rw-r--r--   0        0        0      306 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/RemoteStopTransaction.json
+-rw-r--r--   0        0        0      427 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/RemoteStopTransactionResponse.json
+-rw-r--r--   0        0        0      704 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ReserveNow.json
+-rw-r--r--   0        0        0      502 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ReserveNowResponse.json
+-rw-r--r--   0        0        0      398 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/Reset.json
+-rw-r--r--   0        0        0      411 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/ResetResponse.json
+-rw-r--r--   0        0        0      464 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SecurityEventNotification.json
+-rw-r--r--   0        0        0      177 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SecurityEventNotificationResponse.json
+-rw-r--r--   0        0        0     2146 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SendLocalList.json
+-rw-r--r--   0        0        0      484 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SendLocalListResponse.json
+-rw-r--r--   0        0        0     4310 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SetChargingProfile.json
+-rw-r--r--   0        0        0      456 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SetChargingProfileResponse.json
+-rw-r--r--   0        0        0      287 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SignCertificate.json
+-rw-r--r--   0        0        0      483 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SignCertificateResponse.json
+-rw-r--r--   0        0        0      876 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SignedFirmwareStatusNotification.json
+-rw-r--r--   0        0        0      184 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SignedFirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0     1212 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SignedUpdateFirmware.json
+-rw-r--r--   0        0        0      590 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json
+-rw-r--r--   0        0        0      676 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/StartTransaction.json
+-rw-r--r--   0        0        0     1162 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/StartTransactionResponse.json
+-rw-r--r--   0        0        0     1805 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/StatusNotification.json
+-rw-r--r--   0        0        0      183 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/StatusNotificationResponse.json
+-rw-r--r--   0        0        0     7313 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/StopTransaction.json
+-rw-r--r--   0        0        0     1023 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/StopTransactionResponse.json
+-rw-r--r--   0        0        0      678 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/TriggerMessage.json
+-rw-r--r--   0        0        0      454 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/TriggerMessageResponse.json
+-rw-r--r--   0        0        0      296 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/UnlockConnector.json
+-rw-r--r--   0        0        0      457 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/UnlockConnectorResponse.json
+-rw-r--r--   0        0        0      572 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/UpdateFirmware.json
+-rw-r--r--   0        0        0      179 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v16/schemas/UpdateFirmwareResponse.json
+-rw-r--r--   0        0        0      189 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/__init__.py
+-rw-r--r--   0        0        0    34073 2024-05-07 10:02:50.787007 ocpp-1.0.0/ocpp/v201/call.py
+-rw-r--r--   0        0        0    32301 2024-02-05 14:06:46.101172 ocpp-1.0.0/ocpp/v201/call_result.py
+-rw-r--r--   0        0        0    22081 2024-05-07 10:02:50.791008 ocpp-1.0.0/ocpp/v201/datatypes.py
+-rw-r--r--   0        0        0    80113 2024-05-07 10:02:50.791008 ocpp-1.0.0/ocpp/v201/enums.py
+-rwxr-xr-x   0        0        0     4203 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/AuthorizeRequest.json
+-rwxr-xr-x   0        0        0     7208 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/AuthorizeResponse.json
+-rwxr-xr-x   0        0        0     3161 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/BootNotificationRequest.json
+-rwxr-xr-x   0        0        0     2270 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/BootNotificationResponse.json
+-rwxr-xr-x   0        0        0      775 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/CancelReservationRequest.json
+-rwxr-xr-x   0        0        0     1758 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/CancelReservationResponse.json
+-rwxr-xr-x   0        0        0     1914 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/CertificateSignedRequest.json
+-rwxr-xr-x   0        0        0     1752 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/CertificateSignedResponse.json
+-rwxr-xr-x   0        0        0     1811 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ChangeAvailabilityRequest.json
+-rwxr-xr-x   0        0        0     1783 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ChangeAvailabilityResponse.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearCacheRequest.json
+-rwxr-xr-x   0        0        0     1735 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearCacheResponse.json
+-rwxr-xr-x   0        0        0     2574 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearChargingProfileRequest.json
+-rwxr-xr-x   0        0        0     1752 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearChargingProfileResponse.json
+-rwxr-xr-x   0        0        0      787 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearDisplayMessageRequest.json
+-rwxr-xr-x   0        0        0     1735 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearDisplayMessageResponse.json
+-rwxr-xr-x   0        0        0      865 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearVariableMonitoringRequest.json
+-rwxr-xr-x   0        0        0     2327 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearVariableMonitoringResponse.json
+-rwxr-xr-x   0        0        0     1087 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearedChargingLimitRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/ClearedChargingLimitResponse.json
+-rwxr-xr-x   0        0        0     1121 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/CostUpdatedRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/CostUpdatedResponse.json
+-rwxr-xr-x   0        0        0     4659 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/CustomerInformationRequest.json
+-rwxr-xr-x   0        0        0     1740 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/CustomerInformationResponse.json
+-rwxr-xr-x   0        0        0     1101 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/DataTransferRequest.json
+-rwxr-xr-x   0        0        0     1869 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/DataTransferResponse.json
+-rwxr-xr-x   0        0        0     1808 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/DeleteCertificateRequest.json
+-rwxr-xr-x   0        0        0     1747 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/DeleteCertificateResponse.json
+-rwxr-xr-x   0        0        0     1539 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json
+-rwxr-xr-x   0        0        0     1424 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/Get15118EVCertificateRequest.json
+-rwxr-xr-x   0        0        0     1915 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/Get15118EVCertificateResponse.json
+-rwxr-xr-x   0        0        0     1105 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetBaseReportRequest.json
+-rwxr-xr-x   0        0        0     1794 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetBaseReportResponse.json
+-rwxr-xr-x   0        0        0     1957 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetCertificateStatusRequest.json
+-rwxr-xr-x   0        0        0     2089 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetCertificateStatusResponse.json
+-rwxr-xr-x   0        0        0     3622 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetChargingProfilesRequest.json
+-rwxr-xr-x   0        0        0     1859 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetChargingProfilesResponse.json
+-rwxr-xr-x   0        0        0     1329 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetCompositeScheduleRequest.json
+-rwxr-xr-x   0        0        0     5095 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetCompositeScheduleResponse.json
+-rwxr-xr-x   0        0        0     1874 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetDisplayMessagesRequest.json
+-rwxr-xr-x   0        0        0     1841 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetDisplayMessagesResponse.json
+-rwxr-xr-x   0        0        0     1204 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json
+-rwxr-xr-x   0        0        0     3997 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetLocalListVersionRequest.json
+-rwxr-xr-x   0        0        0      840 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetLocalListVersionResponse.json
+-rwxr-xr-x   0        0        0     2802 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetLogRequest.json
+-rwxr-xr-x   0        0        0     1954 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetLogResponse.json
+-rwxr-xr-x   0        0        0     4175 2023-09-27 14:02:09.711739 ocpp-1.0.0/ocpp/v201/schemas/GetMonitoringReportRequest.json
+-rwxr-xr-x   0        0        0     1800 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/GetMonitoringReportResponse.json
+-rwxr-xr-x   0        0        0     4143 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/GetReportRequest.json
+-rwxr-xr-x   0        0        0     1800 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/GetReportResponse.json
+-rwxr-xr-x   0        0        0      784 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/GetTransactionStatusRequest.json
+-rwxr-xr-x   0        0        0      910 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/GetTransactionStatusResponse.json
+-rwxr-xr-x   0        0        0     3931 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/GetVariablesRequest.json
+-rwxr-xr-x   0        0        0     5581 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/GetVariablesResponse.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/HeartbeatRequest.json
+-rwxr-xr-x   0        0        0      802 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/HeartbeatResponse.json
+-rwxr-xr-x   0        0        0     1226 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/InstallCertificateRequest.json
+-rwxr-xr-x   0        0        0     1751 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/InstallCertificateResponse.json
+-rwxr-xr-x   0        0        0     1361 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/LogStatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/LogStatusNotificationResponse.json
+-rwxr-xr-x   0        0        0     7709 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/MeterValuesRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/MeterValuesResponse.json
+-rwxr-xr-x   0        0        0    11333 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyChargingLimitRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyChargingLimitResponse.json
+-rwxr-xr-x   0        0        0     1542 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyCustomerInformationRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyCustomerInformationResponse.json
+-rwxr-xr-x   0        0        0     6512 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json
+-rwxr-xr-x   0        0        0     5943 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json
+-rwxr-xr-x   0        0        0     1870 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json
+-rwxr-xr-x   0        0        0    10370 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json
+-rwxr-xr-x   0        0        0     1780 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json
+-rwxr-xr-x   0        0        0     6614 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyEventRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyEventResponse.json
+-rwxr-xr-x   0        0        0     7005 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyMonitoringReportRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyMonitoringReportResponse.json
+-rwxr-xr-x   0        0        0     8608 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyReportRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/NotifyReportResponse.json
+-rwxr-xr-x   0        0        0     1668 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/PublishFirmwareRequest.json
+-rwxr-xr-x   0        0        0     1691 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/PublishFirmwareResponse.json
+-rwxr-xr-x   0        0        0     1631 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json
+-rwxr-xr-x   0        0        0    14700 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/ReportChargingProfilesRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/ReportChargingProfilesResponse.json
+-rwxr-xr-x   0        0        0    15964 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/RequestStartTransactionRequest.json
+-rwxr-xr-x   0        0        0     2080 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/RequestStartTransactionResponse.json
+-rwxr-xr-x   0        0        0      844 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/RequestStopTransactionRequest.json
+-rwxr-xr-x   0        0        0     1760 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/RequestStopTransactionResponse.json
+-rwxr-xr-x   0        0        0     1133 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/ReservationStatusUpdateRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/ReservationStatusUpdateResponse.json
+-rwxr-xr-x   0        0        0     3649 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/ReserveNowRequest.json
+-rwxr-xr-x   0        0        0     1758 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/ReserveNowResponse.json
+-rwxr-xr-x   0        0        0     1144 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/ResetRequest.json
+-rwxr-xr-x   0        0        0     1730 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/ResetResponse.json
+-rwxr-xr-x   0        0        0     1120 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SecurityEventNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SecurityEventNotificationResponse.json
+-rwxr-xr-x   0        0        0     7733 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SendLocalListRequest.json
+-rwxr-xr-x   0        0        0     1810 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SendLocalListResponse.json
+-rwxr-xr-x   0        0        0    13730 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetChargingProfileRequest.json
+-rwxr-xr-x   0        0        0     1913 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetChargingProfileResponse.json
+-rwxr-xr-x   0        0        0     5989 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetDisplayMessageRequest.json
+-rwxr-xr-x   0        0        0     1848 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetDisplayMessageResponse.json
+-rwxr-xr-x   0        0        0     1005 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetMonitoringBaseRequest.json
+-rwxr-xr-x   0        0        0     1789 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetMonitoringBaseResponse.json
+-rwxr-xr-x   0        0        0     2087 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetMonitoringLevelRequest.json
+-rwxr-xr-x   0        0        0     1718 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetMonitoringLevelResponse.json
+-rwxr-xr-x   0        0        0     7613 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetNetworkProfileRequest.json
+-rwxr-xr-x   0        0        0     1710 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetNetworkProfileResponse.json
+-rwxr-xr-x   0        0        0     5959 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetVariableMonitoringRequest.json
+-rwxr-xr-x   0        0        0     6923 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetVariableMonitoringResponse.json
+-rwxr-xr-x   0        0        0     4272 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetVariablesRequest.json
+-rwxr-xr-x   0        0        0     5035 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SetVariablesResponse.json
+-rwxr-xr-x   0        0        0     1481 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SignCertificateRequest.json
+-rwxr-xr-x   0        0        0     1699 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/SignCertificateResponse.json
+-rwxr-xr-x   0        0        0     1570 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/StatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/StatusNotificationResponse.json
+-rwxr-xr-x   0        0        0    14824 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/TransactionEventRequest.json
+-rwxr-xr-x   0        0        0     7606 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/TransactionEventResponse.json
+-rwxr-xr-x   0        0        0     1996 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/TriggerMessageRequest.json
+-rwxr-xr-x   0        0        0     1772 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/TriggerMessageResponse.json
+-rwxr-xr-x   0        0        0      970 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/UnlockConnectorRequest.json
+-rwxr-xr-x   0        0        0     1776 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/UnlockConnectorResponse.json
+-rwxr-xr-x   0        0        0      837 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/UnpublishFirmwareRequest.json
+-rwxr-xr-x   0        0        0     1059 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/UnpublishFirmwareResponse.json
+-rwxr-xr-x   0        0        0     2765 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/UpdateFirmwareRequest.json
+-rwxr-xr-x   0        0        0     1824 2023-09-27 14:02:09.715739 ocpp-1.0.0/ocpp/v201/schemas/UpdateFirmwareResponse.json
+-rw-r--r--   0        0        0     1576 2024-05-14 14:28:13.192376 ocpp-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7781 1970-01-01 00:00:00.000000 ocpp-1.0.0/PKG-INFO
```

### Comparing `ocpp-0.9.0/LICENSE` & `ocpp-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/README.rst` & `ocpp-1.0.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-.. image:: https://circleci.com/gh/mobilityhouse/ocpp/tree/master.svg?style=svg
-   :target: https://circleci.com/gh/mobilityhouse/ocpp/tree/master
+.. image:: https://github.com/mobilityhouse/ocpp/actions/workflows/pull-request.yml/badge.svg?style=svg
+   :target: https://github.com/mobilityhouse/ocpp/actions/workflows/pull-request.yml
 
 .. image:: https://img.shields.io/pypi/pyversions/ocpp.svg
    :target: https://pypi.org/project/ocpp/
 
 .. image:: https://img.shields.io/readthedocs/ocpp.svg
    :target: https://ocpp.readthedocs.io/en/latest/
 
 OCPP
 ----
 
 Python package implementing the JSON version of the Open Charge Point Protocol
-(OCPP). Currently OCPP 1.6 (errata v4), OCPP 2.0 and OCPP 2.0.1 (Final Version)
+(OCPP). Currently OCPP 1.6 (errata v4), OCPP 2.0.1 (Edition 2 FINAL, 2022-12-15)
 are supported.
 
 You can find the documentation on `rtd`_.
 
+The purpose of this library is to provide the building blocks to construct a
+charging station/charge point and/or charging station management system
+(CSMS)/central system. The library does not provide a completed solution, as any
+implementation is specific for its intended use. The documents in this library
+should be inspected, as these documents provided guidance on how best to
+build a complete solution.
+
+Note: "OCPP 2.0.1 contains fixes for all the known issues, to date, not only
+the fixes to the messages. This version replaces OCPP 2.0. OCA advises
+implementers of OCPP to no longer implement OCPP 2.0 and only use version
+2.0.1 going forward."
+
 Installation
 ------------
 
 You can either the project install from Pypi:
 
 .. code-block:: bash
 
@@ -30,67 +42,71 @@
 .. code-block:: bash
 
    $ pip install .
 
 Quick start
 -----------
 
-Below you can find examples on how to create a simple OCPP 2.0 central system as
-well as an OCPP 2.0 charge point.
+Below you can find examples on how to create a simple OCPP 1.6 or 2.0.1 Central
+System/CSMS as well as the respective OCPP 1.6 or 2.0.1
+Charging Station/Charge Point.
 
 .. note::
 
    To run these examples the dependency websockets_ is required! Install it by running:
 
    .. code-block:: bash
 
       $ pip install websockets
 
-Central system
-~~~~~~~~~~~~~~
+Charging Station Management System (CSMS) / Central System
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The code snippet below creates a simple OCPP 2.0 central system which is able
-to handle BootNotification calls. You can find a detailed explanation of the
-code in the `Central System documentation_`.
+The code snippet below creates a simple OCPP 2.0.1 CSMS which
+is able to handle BootNotification calls. You can find a detailed explanation of the
+code in the `Central System documentation`_.
 
 
 .. code-block:: python
 
     import asyncio
     import logging
     import websockets
     from datetime import datetime
 
     from ocpp.routing import on
     from ocpp.v201 import ChargePoint as cp
     from ocpp.v201 import call_result
+    from ocpp.v201.enums import RegistrationStatusType
 
     logging.basicConfig(level=logging.INFO)
 
 
     class ChargePoint(cp):
         @on('BootNotification')
         async def on_boot_notification(self, charging_station, reason, **kwargs):
             return call_result.BootNotificationPayload(
                 current_time=datetime.utcnow().isoformat(),
                 interval=10,
-                status='Accepted'
+                status=RegistrationStatusType.accepted
             )
 
 
     async def on_connect(websocket, path):
         """ For every new charge point that connects, create a ChargePoint
         instance and start listening for messages.
         """
         try:
             requested_protocols = websocket.request_headers[
                 'Sec-WebSocket-Protocol']
         except KeyError:
             logging.info("Client hasn't requested any Subprotocol. "
                      "Closing Connection")
+            return await websocket.close()
+
         if websocket.subprotocol:
             logging.info("Protocols Matched: %s", websocket.subprotocol)
         else:
             # In the websockets lib if no subprotocols are supported by the
             # client and the server, it proceeds without a subprotocol,
             # so we have to manually close the connection.
             logging.warning('Protocols Mismatched | Expected Subprotocols: %s,'
@@ -114,58 +130,59 @@
         )
         logging.info("WebSocket Server Started")
         await server.wait_closed()
 
     if __name__ == '__main__':
         asyncio.run(main())
 
-Charge point
-~~~~~~~~~~~~
+Charging Station / Charge point
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
     import asyncio
+
+    from ocpp.v201.enums import RegistrationStatusType
     import logging
     import websockets
 
     from ocpp.v201 import call
     from ocpp.v201 import ChargePoint as cp
 
     logging.basicConfig(level=logging.INFO)
 
 
     class ChargePoint(cp):
 
-       async def send_boot_notification(self):
-           request = call.BootNotificationPayload(
-                   charging_station={
-                       'model': 'Wallbox XYZ',
-                       'vendor_name': 'anewone'
-                   },
-                   reason="PowerUp"
-           )
-           response = await self.call(request)
+        async def send_boot_notification(self):
+            request = call.BootNotificationPayload(
+                charging_station={
+                    'model': 'Wallbox XYZ',
+                    'vendor_name': 'anewone'
+                },
+                reason="PowerUp"
+            )
+            response = await self.call(request)
 
-           if response.status == 'Accepted':
-               print("Connected to central system.")
+            if response.status == RegistrationStatusType.accepted:
+                print("Connected to central system.")
 
 
     async def main():
-       async with websockets.connect(
-           'ws://localhost:9000/CP_1',
-            subprotocols=['ocpp2.0.1']
-       ) as ws:
+        async with websockets.connect(
+                'ws://localhost:9000/CP_1',
+                subprotocols=['ocpp2.0.1']
+        ) as ws:
+            cp = ChargePoint('CP_1', ws)
 
-           cp = ChargePoint('CP_1', ws)
-
-           await asyncio.gather(cp.start(), cp.send_boot_notification())
+            await asyncio.gather(cp.start(), cp.send_boot_notification())
 
 
     if __name__ == '__main__':
-       asyncio.run(main())
+        asyncio.run(main())
 
 Debugging
 ---------
 
 Python's default log level is `logging.WARNING`. As result most of the logs
 generated by this package are discarded. To see the log output of this package
 lower the log level to `logging.DEBUG`.
```

### Comparing `ocpp-0.9.0/ocpp/charge_point.py` & `ocpp-1.0.0/ocpp/charge_point.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import asyncio
 import inspect
 import logging
-import uuid
 import re
 import time
-from dataclasses import asdict
+import uuid
+from dataclasses import Field, asdict, is_dataclass
+from typing import Any, Dict, List, Union, get_args, get_origin
 
+from ocpp.exceptions import NotImplementedError, NotSupportedError, OCPPError
+from ocpp.messages import Call, MessageType, unpack, validate_payload
 from ocpp.routing import create_route_map
-from ocpp.messages import Call, validate_payload, MessageType
-from ocpp.exceptions import OCPPError, NotImplementedError
-from ocpp.messages import unpack
 
-LOGGER = logging.getLogger('ocpp')
+LOGGER = logging.getLogger("ocpp")
 
 
 def camel_to_snake_case(data):
     """
     Convert all keys of all dictionaries inside the given argument from
     camelCase to snake_case.
 
     Inspired by: https://stackoverflow.com/a/1176023/1073222
 
     """
     if isinstance(data, dict):
         snake_case_dict = {}
         for key, value in data.items():
-            s1 = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', key)
-            key = re.sub('([a-z0-9])([A-Z])', r'\1_\2', s1).lower()
+            key = key.replace("ocppCSMS", "ocpp_csms")
+            key = key.replace("V2X", "_v2x")
+            key = key.replace("V2X", "_v2x").replace("V2G", "_v2g")
+            s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", key)
+            key = re.sub("([a-z0-9])([A-Z])(?=\\S)", r"\1_\2", s1).lower()
 
             snake_case_dict[key] = camel_to_snake_case(value)
 
         return snake_case_dict
 
     if isinstance(data, list):
         snake_case_list = []
@@ -40,51 +43,160 @@
         return snake_case_list
 
     return data
 
 
 def snake_to_camel_case(data):
     """
-    Convert all keys of a all dictionaries inside given argument from
+    Convert all keys of all dictionaries inside given argument from
     snake_case to camelCase.
 
     Inspired by: https://stackoverflow.com/a/19053800/1073222
     """
     if isinstance(data, dict):
         camel_case_dict = {}
         for key, value in data.items():
-            components = key.split('_')
-            key = components[0] + ''.join(x.title() for x in components[1:])
+            key = key.replace("soc", "SoC")
+            key = key.replace("_v2x", "V2X")
+            key = key.replace("ocpp_csms", "ocppCSMS")
+            key = key.replace("_url", "URL")
+            key = key.replace("soc", "SoC").replace("_SoCket", "Socket")
+            key = key.replace("_v2x", "V2X")
+            key = key.replace("soc_limit_reached", "SOCLimitReached")
+            key = key.replace("_v2x", "V2X").replace("_v2g", "V2G")
+            components = key.split("_")
+            key = components[0] + "".join(x[:1].upper() + x[1:] for x in components[1:])
             camel_case_dict[key] = snake_to_camel_case(value)
 
         return camel_case_dict
 
     if isinstance(data, list):
         camel_case_list = []
         for value in data:
             camel_case_list.append(snake_to_camel_case(value))
 
         return camel_case_list
 
     return data
 
 
-def remove_nones(dict_to_scan):
-    dict_to_scan = {
-        k: v for k, v in dict_to_scan.items()
-        if v is not None
+def _is_dataclass_instance(input: Any) -> bool:
+    """Verify if given `input` is a dataclass."""
+    return is_dataclass(input) and not isinstance(input, type)
+
+
+def _is_optional_field(field: Field) -> bool:
+    """Verify if given `field` allows `None` as value.
+
+    The fields `schema` and `host` on the following class would return `False`.
+    While the fields `post` and `query` return `True`.
+
+        @dataclass
+        class URL:
+            schema: str,
+            host: str,
+            post: Optional[str],
+            query: Union[None, str]
+
+    """
+    return get_origin(field.type) is Union and type(None) in get_args(field.type)
+
+
+def serialize_as_dict(dataclass):
+    """Serialize the given `dataclass` as a `dict` recursively.
+
+    @dataclass
+    class StatusInfoType:
+        reason_code: str
+        additional_info: Optional[str] = None
+
+    with_additional_info = StatusInfoType(
+        reason="Unknown",
+        additional_info="More details"
+    )
+
+    assert serialize_as_dict(with_additional_info) == {
+        'reason': 'Unknown',
+        'additional_info': 'More details',
     }
-    return dict_to_scan
+
+    without_additional_info = StatusInfoType(reason="Unknown")
+
+    assert serialize_as_dict(with_additional_info) == {
+        'reason': 'Unknown',
+        'additional_info': None,
+    }
+
+    """
+    serialized = asdict(dataclass)
+
+    for field in dataclass.__dataclass_fields__.values():
+
+        value = getattr(dataclass, field.name)
+        if _is_dataclass_instance(value):
+            serialized[field.name] = serialize_as_dict(value)
+            continue
+
+        if isinstance(value, list):
+            for item in value:
+                if _is_dataclass_instance(item):
+                    serialized[field.name] = [serialize_as_dict(item)]
+
+    return serialized
+
+
+def remove_nones(data: Union[List, Dict]) -> Union[List, Dict]:
+    if isinstance(data, dict):
+        return {k: remove_nones(v) for k, v in data.items() if v is not None}
+
+    elif isinstance(data, list):
+        return [remove_nones(v) for v in data if v is not None]
+
+    return data
+
+
+def _raise_key_error(action, version):
+    """
+    Checks whether a keyerror returned by _handle_call
+    is supported by the OCPP version or is simply
+    not implemented by the server/client and raises
+    the appropriate error.
+    """
+
+    from ocpp.v16.enums import Action as v16_Action
+    from ocpp.v201.enums import Action as v201_Action
+
+    if version == "1.6":
+        if hasattr(v16_Action, action):
+            raise NotImplementedError(
+                details={"cause": f"No handler for {action} registered."}
+            )
+        else:
+            raise NotSupportedError(
+                details={"cause": f"{action} not supported by OCPP{version}."}
+            )
+    elif version in ["2.0", "2.0.1"]:
+        if hasattr(v201_Action, action):
+            raise NotImplementedError(
+                details={"cause": f"No handler for {action} registered."}
+            )
+        else:
+            raise NotSupportedError(
+                details={"cause": f"{action} not supported by OCPP{version}."}
+            )
+
+    return
 
 
 class ChargePoint:
     """
     Base Element containing all the necessary OCPP1.6J messages for messages
     initiated and received by the Central System
     """
+
     def __init__(self, id, connection, response_timeout=30):
         """
 
         Args:
 
             charger_id (str): ID of the charger.
             connection: Connection to CP.
@@ -117,118 +229,139 @@
         # uuid.uuid4() is used, but it can be changed. This is meant primarily
         # for testing purposes to have predictable unique ids.
         self._unique_id_generator = uuid.uuid4
 
     async def start(self):
         while True:
             message = await self._connection.recv()
-            LOGGER.info('%s: receive message %s', self.id, message)
+            LOGGER.info("%s: receive message %s", self.id, message)
 
             await self.route_message(message)
 
     async def route_message(self, raw_msg):
         """
         Route a message received from a CP.
 
         If the message is a of type Call the corresponding hooks are executed.
         If the message is of type CallResult or CallError the message is passed
         to the call() function via the response_queue.
         """
         try:
             msg = unpack(raw_msg)
         except OCPPError as e:
-            LOGGER.exception("Unable to parse message: '%s', it doesn't seem "
-                             "to be valid OCPP: %s", raw_msg, e)
+            LOGGER.exception(
+                "Unable to parse message: '%s', it doesn't seem "
+                "to be valid OCPP: %s",
+                raw_msg,
+                e,
+            )
             return
 
         if msg.message_type_id == MessageType.Call:
-            await self._handle_call(msg)
+            try:
+                await self._handle_call(msg)
+            except OCPPError as error:
+                LOGGER.exception("Error while handling request '%s'", msg)
+                response = msg.create_call_error(error).to_json()
+                await self._send(response)
 
-        elif msg.message_type_id in \
-                [MessageType.CallResult, MessageType.CallError]:
+        elif msg.message_type_id in [MessageType.CallResult, MessageType.CallError]:
             self._response_queue.put_nowait(msg)
 
     async def _handle_call(self, msg):
         """
         Execute all hooks installed for based on the Action of the message.
 
         First the '_on_action' hook is executed and its response is returned to
         the client. If there is no '_on_action' hook for Action in the message
-        a CallError with a NotImplemtendError is returned.
+        a CallError with a NotImplementedError is returned. If the Action is
+        not supported by the OCPP version a NotSupportedError is returned.
 
         Next the '_after_action' hook is executed.
 
         """
         try:
             handlers = self.route_map[msg.action]
         except KeyError:
-            raise NotImplementedError(f"No handler for '{msg.action}' "
-                                      "registered.")
+            _raise_key_error(msg.action, self._ocpp_version)
+            return
 
-        if not handlers.get('_skip_schema_validation', False):
+        if not handlers.get("_skip_schema_validation", False):
             validate_payload(msg, self._ocpp_version)
-
         # OCPP uses camelCase for the keys in the payload. It's more pythonic
         # to use snake_case for keyword arguments. Therefore the keys must be
         # 'translated'. Some examples:
         #
         # * chargePointVendor becomes charge_point_vendor
         # * firmwareVersion becomes firmwareVersion
         snake_case_payload = camel_to_snake_case(msg.payload)
 
         try:
-            handler = handlers['_on_action']
+            handler = handlers["_on_action"]
         except KeyError:
-            raise NotImplementedError(f"No handler for '{msg.action}' "
-                                      "registered.")
-
+            _raise_key_error(msg.action, self._ocpp_version)
+        handler_signature = inspect.signature(handler)
+        call_unique_id_required = "call_unique_id" in handler_signature.parameters
         try:
-            response = handler(**snake_case_payload)
+            # call_unique_id should be passed as kwarg only if is defined explicitly
+            # in the handler signature
+            if call_unique_id_required:
+                response = handler(**snake_case_payload, call_unique_id=msg.unique_id)
+            else:
+                response = handler(**snake_case_payload)
             if inspect.isawaitable(response):
                 response = await response
         except Exception as e:
             LOGGER.exception("Error while handling request '%s'", msg)
             response = msg.create_call_error(e).to_json()
             await self._send(response)
 
             return
 
-        temp_response_payload = asdict(response)
+        temp_response_payload = serialize_as_dict(response)
 
         # Remove nones ensures that we strip out optional arguments
         # which were not set and have a default value of None
         response_payload = remove_nones(temp_response_payload)
 
         # The response payload must be 'translated' from snake_case to
         # camelCase. So:
         #
         # * charge_point_vendor becomes chargePointVendor
         # * firmware_version becomes firmwareVersion
         camel_case_payload = snake_to_camel_case(response_payload)
 
         response = msg.create_call_result(camel_case_payload)
 
-        if not handlers.get('_skip_schema_validation', False):
+        if not handlers.get("_skip_schema_validation", False):
             validate_payload(response, self._ocpp_version)
 
         await self._send(response.to_json())
 
         try:
-            handler = handlers['_after_action']
+            handler = handlers["_after_action"]
+            handler_signature = inspect.signature(handler)
+            call_unique_id_required = "call_unique_id" in handler_signature.parameters
+            # call_unique_id should be passed as kwarg only if is defined explicitly
+            # in the handler signature
+            if call_unique_id_required:
+                response = handler(**snake_case_payload, call_unique_id=msg.unique_id)
+            else:
+                response = handler(**snake_case_payload)
             # Create task to avoid blocking when making a call inside the
             # after handler
-            response = handler(**snake_case_payload)
             if inspect.isawaitable(response):
                 asyncio.ensure_future(response)
         except KeyError:
             # '_on_after' hooks are not required. Therefore ignore exception
             # when no '_on_after' hook is installed.
             pass
+        return response
 
-    async def call(self, payload, suppress=True):
+    async def call(self, payload, suppress=True, unique_id=None):
         """
         Send Call message to client and return payload of response.
 
         The given payload is transformed into a Call object by looking at the
         type of the payload. A payload of type BootNotificationPayload will
         turn in a Call with Action BootNotification, a HeartbeatPayload will
         result in a Call with Action Heartbeat etc.
@@ -242,32 +375,41 @@
 
         Suppress is used to maintain backwards compatibility. When set to True,
         if response is a CallError, then this call will be suppressed. When
         set to False, an exception will be raised for users to handle this
         CallError.
 
         """
-        camel_case_payload = snake_to_camel_case(asdict(payload))
+        camel_case_payload = snake_to_camel_case(serialize_as_dict(payload))
+
+        unique_id = (
+            unique_id if unique_id is not None else str(self._unique_id_generator())
+        )
+
+        action_name = payload.__class__.__name__
+        # Due to deprecated call and callresults, remove in the future.
+        if "Payload" in payload.__class__.__name__:
+            action_name = payload.__class__.__name__[:-7]
 
         call = Call(
-            unique_id=str(self._unique_id_generator()),
-            action=payload.__class__.__name__[:-7],
-            payload=remove_nones(camel_case_payload)
+            unique_id=unique_id,
+            action=action_name,
+            payload=remove_nones(camel_case_payload),
         )
 
         validate_payload(call, self._ocpp_version)
 
         # Use a lock to prevent make sure that only 1 message can be send at a
         # a time.
         async with self._call_lock:
             await self._send(call.to_json())
             try:
-                response = \
-                    await self._get_specific_response(call.unique_id,
-                                                      self._response_timeout)
+                response = await self._get_specific_response(
+                    call.unique_id, self._response_timeout
+                )
             except asyncio.TimeoutError:
                 raise asyncio.TimeoutError(
                     f"Waited {self._response_timeout}s for response on "
                     f"{call.to_json()}."
                 )
 
         if response.message_type_id == MessageType.CallError:
@@ -291,26 +433,25 @@
     async def _get_specific_response(self, unique_id, timeout):
         """
         Return response with given unique ID or raise an asyncio.TimeoutError.
         """
         wait_until = time.time() + timeout
         try:
             # Wait for response of the Call message.
-            response = await asyncio.wait_for(self._response_queue.get(),
-                                              timeout)
+            response = await asyncio.wait_for(self._response_queue.get(), timeout)
         except asyncio.TimeoutError:
             raise
 
         if response.unique_id == unique_id:
             return response
 
-        LOGGER.error('Ignoring response with unknown unique id: %s', response)
+        LOGGER.error("Ignoring response with unknown unique id: %s", response)
         timeout_left = wait_until - time.time()
 
         if timeout_left < 0:
             raise asyncio.TimeoutError
 
         return await self._get_specific_response(unique_id, timeout_left)
 
     async def _send(self, message):
-        LOGGER.info('%s: send %s', self.id, message)
+        LOGGER.info("%s: send %s", self.id, message)
         await self._connection.send(message)
```

### Comparing `ocpp-0.9.0/ocpp/messages.py` & `ocpp-1.0.0/ocpp/messages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 """ Module containing classes that model the several OCPP messages types. It
 also contain some helper functions for packing and unpacking messages.  """
-import os
-import json
+from __future__ import annotations
+
 import decimal
-import warnings
-from typing import Callable, Dict
+import json
+import os
 from dataclasses import asdict, is_dataclass
+from typing import Callable, Dict, Union
 
 from jsonschema import Draft4Validator
 from jsonschema.exceptions import ValidationError as SchemaValidationError
 
-from ocpp.exceptions import (OCPPError, FormatViolationError,
-                             PropertyConstraintViolationError,
-                             ProtocolError, ValidationError,
-                             UnknownCallErrorCodeError)
+from ocpp.exceptions import (
+    FormatViolationError,
+    NotImplementedError,
+    OCPPError,
+    PropertyConstraintViolationError,
+    ProtocolError,
+    TypeConstraintViolationError,
+    UnknownCallErrorCodeError,
+    ValidationError,
+)
 
-_schemas: Dict[str, Dict] = {}
 _validators: Dict[str, Draft4Validator] = {}
 
 
 class _DecimalEncoder(json.JSONEncoder):
-    """ Encode values of type `decimal.Decimal` using 1 decimal point.
+    """Encode values of type `decimal.Decimal` using 1 decimal point.
 
     A custom encoder is required because `json.dumps()` cannot encode a value
     of type decimal.Decimal. This raises a TypeError:
 
         >>> import decimal
         >>> import json
         >>> >>> json.dumps(decimal.Decimal(3))
@@ -39,22 +45,30 @@
           File "/home/developer/.pyenv/versions/3.7.0/lib/python3.7/json/encoder.py", line 179, in default
             raise TypeError(f'Object of type {o.__class__.__name__} '
         TypeError: Object of type Decimal is not JSON serializable
 
     This can be prevented by using a custom encoder.
 
     """
+
     def default(self, obj):
         if isinstance(obj, decimal.Decimal):
             return float("%.1f" % obj)
-        return json.JSONEncoder.default(self, obj)
+        try:
+            return json.JSONEncoder.default(self, obj)
+        except TypeError as e:
+            try:
+                return obj.to_json()
+            except AttributeError:
+                raise e
 
 
 class MessageType:
-    """ Number identifying the different types of OCPP messages. """
+    """Number identifying the different types of OCPP messages."""
+
     #: Call identifies a request.
     Call = 2
 
     #: CallResult identifies a successful response.
     CallResult = 3
 
     #: CallError identifies an erroneous response.
@@ -63,143 +77,110 @@
 
 def unpack(msg):
     """
     Unpacks a message into either a Call, CallError or CallResult.
     """
     try:
         msg = json.loads(msg)
-    except json.JSONDecodeError as e:
-        raise FormatViolationError(f'Message is not valid JSON: {e}')
+    except json.JSONDecodeError:
+        raise FormatViolationError(
+            details={"cause": "Message is not valid JSON", "ocpp_message": msg}
+        )
 
     if not isinstance(msg, list):
-        raise ProtocolError("OCPP message hasn't the correct format. It "
-                            f"should be a list, but got {type(msg)} instead")
+        raise ProtocolError(
+            details={
+                "cause": (
+                    "OCPP message hasn't the correct format. It "
+                    f"should be a list, but got '{type(msg)}' "
+                    "instead"
+                )
+            }
+        )
 
     for cls in [Call, CallResult, CallError]:
         try:
             if msg[0] == cls.message_type_id:
                 return cls(*msg[1:])
         except IndexError:
-            raise ProtocolError("Message doesn\'t contain MessageTypeID")
+            raise ProtocolError(
+                details={"cause": "Message does not contain MessageTypeId"}
+            )
+        except TypeError:
+            raise ProtocolError(details={"cause": "Message is missing elements."})
 
-    raise PropertyConstraintViolationError(f"MessageTypeId '{msg[0]}' isn't "
-                                           "valid")
+    raise PropertyConstraintViolationError(
+        details={"cause": f"MessageTypeId '{msg[0]}' isn't valid"}
+    )
 
 
 def pack(msg):
     """
     Returns the JSON representation of a Call, CallError or CallResult.
 
     It just calls the 'to_json()' method of the message. But it is here mainly
     to complement the 'unpack' function of this module.
     """
     return msg.to_json()
 
 
-def get_schema(message_type_id, action, ocpp_version, parse_float=float):
-    """
-    Read schema from disk and return in. Reads will be cached for performance
-    reasons.
-
-    The `parse_float` argument can be used to set the conversion method that
-    is used to parse floats. It must be a callable taking 1 argument. By
-    default it is `float()`, but certain schema's require `decimal.Decimal()`.
-    """
-    warnings.warn(
-        "Depricated as of 0.8.1. Please use `ocpp.messages.get_validator()`."
-    )
-
-    if ocpp_version not in ["1.6", "2.0", "2.0.1"]:
-        raise ValueError
-
-    schemas_dir = 'v' + ocpp_version.replace('.', '')
-
-    schema_name = action
-    if message_type_id == MessageType.CallResult:
-        schema_name += 'Response'
-    elif message_type_id == MessageType.Call:
-        if ocpp_version in ["2.0", "2.0.1"]:
-            schema_name += 'Request'
-
-    if ocpp_version == "2.0":
-        schema_name += '_v1p0'
-
-    dir,  _ = os.path.split(os.path.realpath(__file__))
-    relative_path = f'{schemas_dir}/schemas/{schema_name}.json'
-    path = os.path.join(dir, relative_path)
-
-    if relative_path in _schemas:
-        return _schemas[relative_path]
-
-    # The JSON schemas for OCPP 2.0 start with a byte order mark (BOM)
-    # character. If no encoding is given, reading the schema would fail with:
-    #
-    #     Unexpected UTF-8 BOM (decode using utf-8-sig):
-    with open(path, 'r', encoding='utf-8-sig') as f:
-        data = f.read()
-        _schemas[relative_path] = json.loads(data, parse_float=parse_float)
-
-    return _schemas[relative_path]
-
-
 def get_validator(
-        message_type_id: int,
-        action: str,
-        ocpp_version: str,
-        parse_float: Callable = float
+    message_type_id: int, action: str, ocpp_version: str, parse_float: Callable = float
 ) -> Draft4Validator:
     """
     Read schema from disk and return as `Draft4Validator`. Instances will be
     cached for performance reasons.
 
     The `parse_float` argument can be used to set the conversion method that
     is used to parse floats. It must be a callable taking 1 argument. By
     default it is `float()`, but certain schema's require `decimal.Decimal()`.
     """
     if ocpp_version not in ["1.6", "2.0", "2.0.1"]:
         raise ValueError
 
-    schemas_dir = 'v' + ocpp_version.replace('.', '')
+    schemas_dir = "v" + ocpp_version.replace(".", "")
 
     schema_name = action
     if message_type_id == MessageType.CallResult:
-        schema_name += 'Response'
+        schema_name += "Response"
     elif message_type_id == MessageType.Call:
         if ocpp_version in ["2.0", "2.0.1"]:
-            schema_name += 'Request'
+            schema_name += "Request"
 
     if ocpp_version == "2.0":
-        schema_name += '_v1p0'
+        schema_name += "_v1p0"
 
-    cache_key = schema_name + '_' + ocpp_version
+    cache_key = schema_name + "_" + ocpp_version
     if cache_key in _validators:
         return _validators[cache_key]
 
-    dir,  _ = os.path.split(os.path.realpath(__file__))
-    relative_path = f'{schemas_dir}/schemas/{schema_name}.json'
+    dir, _ = os.path.split(os.path.realpath(__file__))
+    relative_path = f"{schemas_dir}/schemas/{schema_name}.json"
     path = os.path.join(dir, relative_path)
 
     # The JSON schemas for OCPP 2.0 start with a byte order mark (BOM)
     # character. If no encoding is given, reading the schema would fail with:
     #
     #     Unexpected UTF-8 BOM (decode using utf-8-sig):
-    with open(path, 'r', encoding='utf-8-sig') as f:
+    with open(path, "r", encoding="utf-8-sig") as f:
         data = f.read()
         validator = Draft4Validator(json.loads(data, parse_float=parse_float))
         _validators[cache_key] = validator
 
     return _validators[cache_key]
 
 
-def validate_payload(message, ocpp_version):
-    """ Validate the payload of the message using JSON schemas. """
+def validate_payload(message: Union[Call, CallResult], ocpp_version: str) -> None:
+    """Validate the payload of the message using JSON schemas."""
     if type(message) not in [Call, CallResult]:
-        raise ValidationError("Payload can't be validated because message "
-                              f"type. It's '{type(message)}', but it should "
-                              "be either 'Call'  or 'CallResult'.")
+        raise ValidationError(
+            "Payload can't be validated because message "
+            f"type. It's '{type(message)}', but it should "
+            "be either 'Call'  or 'CallResult'."
+        )
 
     try:
         # 3 OCPP 1.6 schedules have fields of type floats. The JSON schema
         # defines a certain precision for these fields of 1 decimal. A value of
         # 21.4 is valid, whereas a value if 4.11 is not.
         #
         # The problem is that Python's internal representation of 21.4 might
@@ -209,46 +190,72 @@
         # https://github.com/Julian/jsonschema/issues/247
         #
         # This issue can be fixed by using a different parser for floats than
         # the default one that is used.
         #
         # Both the schema and the payload must be parsed using the different
         # parser for floats.
-        if ocpp_version == '1.6' and (
-            (type(message) == Call and
-                message.action in ['SetChargingProfile', 'RemoteStartTransaction'])  # noqa
-            or
-            (type(message) == CallResult and
-                message.action == 'GetCompositeSchedule')
+        if ocpp_version == "1.6" and (
+            (
+                type(message) == Call
+                and message.action in ["SetChargingProfile", "RemoteStartTransaction"]
+            )  # noqa
+            or (
+                type(message) == CallResult and message.action == "GetCompositeSchedule"
+            )
         ):
             validator = get_validator(
-                message.message_type_id, message.action,
-                ocpp_version, parse_float=decimal.Decimal
+                message.message_type_id,
+                message.action,
+                ocpp_version,
+                parse_float=decimal.Decimal,
             )
 
             message.payload = json.loads(
                 json.dumps(message.payload), parse_float=decimal.Decimal
             )
         else:
             validator = get_validator(
                 message.message_type_id, message.action, ocpp_version
             )
-    except (OSError, json.JSONDecodeError) as e:
-        raise ValidationError("Failed to load validation schema for action "
-                              f"'{message.action}': {e}")
+    except (OSError, json.JSONDecodeError):
+        raise NotImplementedError(
+            details={"cause": f"Failed to validate action: {message.action}"}
+        )
 
     try:
         validator.validate(message.payload)
     except SchemaValidationError as e:
-        raise ValidationError(f"Payload '{message.payload} for action "
-                              f"'{message.action}' is not valid: {e}")
+        if e.validator == "type":
+            raise TypeConstraintViolationError(
+                details={"cause": e.message, "ocpp_message": message}
+            )
+        elif e.validator == "additionalProperties":
+            raise FormatViolationError(
+                details={"cause": e.message, "ocpp_message": message}
+            )
+        elif e.validator == "required":
+            raise ProtocolError(details={"cause": e.message})
+
+        elif e.validator == "maxLength":
+            raise TypeConstraintViolationError(
+                details={"cause": e.message, "ocpp_message": message}
+            ) from e
+        else:
+            raise FormatViolationError(
+                details={
+                    "cause": f"Payload '{message.payload}' for action "
+                    f"'{message.action}' is not valid: {e}",
+                    "ocpp_message": message,
+                }
+            )
 
 
 class Call:
-    """ A Call is a type of message that initiate a request/response sequence.
+    """A Call is a type of message that initiate a request/response sequence.
     Both central systems and charge points can send this message.
 
     From the specification:
 
         A Call always consists of 4 elements: The standard elements
         MessageTypeId and UniqueId, a specific Action that is required on the
         other side and a payload, the arguments to the Action. The syntax of a
@@ -265,36 +272,38 @@
              "BootNotification",
              {
               "chargePointVendor": "VendorX",
               "chargePointModel": "SingleSocketCharger"
              }
             ]
     """
+
     message_type_id = 2
 
     def __init__(self, unique_id, action, payload):
         self.unique_id = unique_id
         self.action = action
         self.payload = payload
 
         if is_dataclass(payload):
             self.payload = asdict(payload)
 
     def to_json(self):
-        """ Return a valid JSON representation of the instance. """
-        return json.dumps([
-            self.message_type_id,
-            self.unique_id,
-            self.action,
-            self.payload,
-        ],
+        """Return a valid JSON representation of the instance."""
+        return json.dumps(
+            [
+                self.message_type_id,
+                self.unique_id,
+                self.action,
+                self.payload,
+            ],
             # By default json.dumps() adds a white space after every separator.
             # By setting the separator manually that can be avoided.
-            separators=(',', ':'),
-            cls=_DecimalEncoder
+            separators=(",", ":"),
+            cls=_DecimalEncoder,
         )
 
     def create_call_result(self, payload):
         call_result = CallResult(self.unique_id, payload)
         call_result.action = self.action
         return call_result
 
@@ -312,22 +321,24 @@
             self.unique_id,
             error_code,
             error_description,
             error_details,
         )
 
     def __repr__(self):
-        return f"<Call - unique_id={self.unique_id}, action={self.action}, " \
-               f"payload={self.payload}>"
+        return (
+            f"<Call - unique_id={self.unique_id}, action={self.action}, "
+            f"payload={self.payload}>"
+        )
 
 
 class CallResult:
     """
     A CallResult is a message indicating that a Call has been handled
-    succesfully.
+    successfully.
 
     From the specification:
 
         A CallResult always consists of 3 elements: The standard elements
         MessageTypeId, UniqueId and a payload, containing the response to the
         Action in the original Call. The syntax of a call looks like this:
 
@@ -343,40 +354,44 @@
               "status":"Accepted",
               "currentTime":"2013-02-01T20:53:32.486Z",
               "heartbeatInterval":300
              }
             ]
 
     """
+
     message_type_id = 3
 
     def __init__(self, unique_id, payload, action=None):
         self.unique_id = unique_id
         self.payload = payload
 
         # Strictly speaking no action is required in a CallResult. But in order
         # to validate the message it is needed.
         self.action = action
 
     def to_json(self):
-        return json.dumps([
-            self.message_type_id,
-            self.unique_id,
-            self.payload,
-        ],
+        return json.dumps(
+            [
+                self.message_type_id,
+                self.unique_id,
+                self.payload,
+            ],
             # By default json.dumps() adds a white space after every separator.
             # By setting the separator manually that can be avoided.
-            separators=(',', ':'),
-            cls=_DecimalEncoder
+            separators=(",", ":"),
+            cls=_DecimalEncoder,
         )
 
     def __repr__(self):
-        return f"<CallResult - unique_id={self.unique_id}, " \
-               f"action={self.action}, " \
-               f"payload={self.payload}>"
+        return (
+            f"<CallResult - unique_id={self.unique_id}, "
+            f"action={self.action}, "
+            f"payload={self.payload}>"
+        )
 
 
 class CallError:
     """
     A CallError is a response to a Call that indicates an error.
 
     From the specification:
@@ -385,47 +400,51 @@
         MessageTypeId and UniqueId, an errorCode string, an errorDescription
         string and an errorDetails object.
 
         The syntax of a call looks like this:
 
             [<MessageTypeId>, "<UniqueId>", "<errorCode>", "<errorDescription>", {<errorDetails>}] # noqa
     """
+
     message_type_id = 4
 
-    def __init__(self, unique_id, error_code, error_description,
-                 error_details=None):
+    def __init__(self, unique_id, error_code, error_description, error_details=None):
         self.unique_id = unique_id
         self.error_code = error_code
         self.error_description = error_description
         self.error_details = error_details
 
     def to_json(self):
-        return json.dumps([
-            self.message_type_id,
-            self.unique_id,
-            self.error_code,
-            self.error_description,
-            self.error_details,
-        ],
+        return json.dumps(
+            [
+                self.message_type_id,
+                self.unique_id,
+                self.error_code,
+                self.error_description,
+                self.error_details,
+            ],
             # By default json.dumps() adds a white space after every separator.
             # By setting the separator manually that can be avoided.
-            separators=(',', ':'),
-            cls=_DecimalEncoder
+            separators=(",", ":"),
+            cls=_DecimalEncoder,
         )
 
     def to_exception(self):
-        """ Return the exception that corresponds to the CallError. """
+        """Return the exception that corresponds to the CallError."""
         for error in OCPPError.__subclasses__():
             if error.code == self.error_code:
                 return error(
-                    description=self.error_description,
-                    details=self.error_details
+                    description=self.error_description, details=self.error_details
                 )
 
-        raise UnknownCallErrorCodeError("Error code '%s' is not defined by the"
-                                        " OCPP specification", self.error_code)
+        raise UnknownCallErrorCodeError(
+            f"Error code '{self.error_code}' is not defined by the"
+            " OCPP specification"
+        )
 
     def __repr__(self):
-        return f"<CallError - unique_id={self.unique_id}, " \
-               f"error_code={self.error_code}, " \
-               f"error_description={self.error_description}, " \
-               f"error_details={self.error_details}>"
+        return (
+            f"<CallError - unique_id={self.unique_id}, "
+            f"error_code={self.error_code}, "
+            f"error_description={self.error_description}, "
+            f"error_details={self.error_details}>"
+        )
```

### Comparing `ocpp-0.9.0/ocpp/routing.py` & `ocpp-1.0.0/ocpp/routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     ```
 
     The decorator takes an optional argument `skip_schema_validation` which
     defaults to False. Setting this argument to `True` will disable schema
     validation of the request and the response of the specific route.
 
     """
+
     def decorator(func):
         @functools.wraps(func)
         def inner(*args, **kwargs):
             return func(*args, **kwargs)
 
         inner._on_action = action
         inner._skip_schema_validation = skip_schema_validation
@@ -52,35 +53,37 @@
             routables.append(func.__name__)
         return inner
 
     return decorator
 
 
 def after(action):
-    """ Function decorator to mark function as hook to post-request hook.
+    """Function decorator to mark function as hook to post-request hook.
 
     This hook's arguments are the data that is in the payload for the specific
     action.
 
     It can be used like so:
 
         @after(Action.BootNotification):
         def after_boot_notification():
             pass
 
     """
+
     def decorator(func):
         @functools.wraps(func)
         def inner(*args, **kwargs):
             return func(*args, **kwargs)
 
         inner._after_action = action
         if func.__name__ not in routables:
             routables.append(func.__name__)
         return inner
+
     return decorator
 
 
 def create_route_map(obj):
     """
     Iterates of all attributes of the class looking for attributes which
     have been decorated by the @on() decorator It returns a dictionary where
@@ -108,28 +111,29 @@
                 '_skip_schema_validation': False,
             },
         }
 
     """
     routes = {}
     for attr_name in routables:
-        for option in ['_on_action', '_after_action']:
+        for option in ["_on_action", "_after_action"]:
             try:
                 attr = getattr(obj, attr_name)
                 action = getattr(attr, option)
 
                 if action not in routes:
                     routes[action] = {}
 
                 # Routes decorated with the `@on()` decorator can be configured
                 # to skip validation of the input and output. For more info see
                 # the docstring of `on()`.
-                if option == '_on_action':
-                    routes[action]['_skip_schema_validation'] = \
-                        getattr(attr, '_skip_schema_validation', False)
+                if option == "_on_action":
+                    routes[action]["_skip_schema_validation"] = getattr(
+                        attr, "_skip_schema_validation", False
+                    )
 
                 routes[action][option] = attr
 
             except AttributeError:
                 continue
 
     return routes
```

### Comparing `ocpp-0.9.0/ocpp/v16/enums.py` & `ocpp-1.0.0/ocpp/v16/enums.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,30 @@
-from enum import Enum
+from warnings import warn
 
+try:
+    # breaking change introduced in python 3.11
+    from enum import StrEnum
+except ImportError:  # pragma: no cover
+    from enum import Enum  # pragma: no cover
 
-class Action(str, Enum):
-    """ An Action is a required part of a Call message. """
+    class StrEnum(str, Enum):  # pragma: no cover
+        pass  # pragma: no cover
+
+
+class Action(StrEnum):
+    """An Action is a required part of a Call message."""
+
+    def __init__(self, *args, **kwargs):
+        warn(
+            message="Action enum contains deprecated members and will be removed in "
+            "the next major release, please use snake case members.",
+            category=DeprecationWarning,
+        )
+
+    # --------- Soon to be deprecated ---------------------
     Authorize = "Authorize"
     BootNotification = "BootNotification"
     CancelReservation = "CancelReservation"
     CertificateSigned = "CertificateSigned"
     ChangeAvailability = "ChangeAvailability"
     ChangeConfiguration = "ChangeConfiguration"
     ClearCache = "ClearCache"
@@ -39,85 +57,127 @@
     StartTransaction = "StartTransaction"
     StatusNotification = "StatusNotification"
     StopTransaction = "StopTransaction"
     TriggerMessage = "TriggerMessage"
     UnlockConnector = "UnlockConnector"
     UpdateFirmware = "UpdateFirmware"
 
+    # --------------------------------------------------------
 
-class AuthorizationStatus(str, Enum):
+    authorize = "Authorize"
+    boot_notification = "BootNotification"
+    cancel_reservation = "CancelReservation"
+    certificate_signed = "CertificateSigned"
+    change_availability = "ChangeAvailability"
+    change_configuration = "ChangeConfiguration"
+    clear_cache = "ClearCache"
+    clear_charging_profile = "ClearChargingProfile"
+    data_transfer = "DataTransfer"
+    delete_certificate = "DeleteCertificate"
+    diagnostics_status_notification = "DiagnosticsStatusNotification"
+    extended_trigger_message = "ExtendedTriggerMessage"
+    firmware_status_notification = "FirmwareStatusNotification"
+    get_composite_schedule = "GetCompositeSchedule"
+    get_configuration = "GetConfiguration"
+    get_diagnostics = "GetDiagnostics"
+    get_installed_certificate_ids = "GetInstalledCertificateIds"
+    get_local_list_version = "GetLocalListVersion"
+    get_log = "GetLog"
+    heartbeat = "Heartbeat"
+    install_certificate = "InstallCertificate"
+    log_status_notification = "LogStatusNotification"
+    meter_values = "MeterValues"
+    remote_start_transaction = "RemoteStartTransaction"
+    remote_stop_transaction = "RemoteStopTransaction"
+    reserve_now = "ReserveNow"
+    reset = "Reset"
+    security_event_notification = "SecurityEventNotification"
+    send_local_list = "SendLocalList"
+    set_charging_profile = "SetChargingProfile"
+    sign_certificate = "SignCertificate"
+    signed_firmware_status_notification = "SignedFirmwareStatusNotification"
+    signed_update_firmware = "SignedUpdateFirmware"
+    start_transaction = "StartTransaction"
+    status_notification = "StatusNotification"
+    stop_transaction = "StopTransaction"
+    trigger_message = "TriggerMessage"
+    unlock_connector = "UnlockConnector"
+    update_firmware = "UpdateFirmware"
+
+
+class AuthorizationStatus(StrEnum):
     """
     Elements that constitute an entry of a Local Authorization List update.
     """
 
     accepted = "Accepted"
     blocked = "Blocked"
     expired = "Expired"
     invalid = "Invalid"
     concurrent_tx = "ConcurrentTx"
 
 
-class AvailabilityStatus(str, Enum):
+class AvailabilityStatus(StrEnum):
     """
     Status returned in response to ChangeAvailability.req.
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
     scheduled = "Scheduled"
 
 
-class AvailabilityType(str, Enum):
+class AvailabilityType(StrEnum):
     """
     Requested availability change in ChangeAvailability.req.
     """
 
     inoperative = "Inoperative"
     operative = "Operative"
 
 
-class CancelReservationStatus(str, Enum):
+class CancelReservationStatus(StrEnum):
     """
     Status in CancelReservation.conf.
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
 
 
-class CertificateSignedStatus(str, Enum):
+class CertificateSignedStatus(StrEnum):
     """
     CertificateSignedStatusEnumType is used by: CertificateSigned.conf
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
 
 
-class CertificateStatus(str, Enum):
+class CertificateStatus(StrEnum):
     """
     CertificateStatusEnumType is used by: InstallCertificate.conf
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
     failed = "Failed"
 
 
-class CertificateUse(str, Enum):
+class CertificateUse(StrEnum):
     """
     CertificateUseEnumType is used by: GetInstalledCertificateIds.req,
     InstallCertificate.req
     """
 
     central_system_root_certificate = "CentralSystemRootCertificate"
     manufacturer_root_certificate = "ManufacturerRootCertificate"
 
 
-class ChargePointErrorCode(str, Enum):
+class ChargePointErrorCode(StrEnum):
     """
     Charge Point status reported in StatusNotification.req.
     """
 
     connector_lock_failure = "ConnectorLockFailure"
     ev_communication_error = "EVCommunicationError"
     ground_failure = "GroundFailure"
@@ -131,34 +191,16 @@
     power_meter_failure = "PowerMeterFailure"
     power_switch_failure = "PowerSwitchFailure"
     reader_failure = "ReaderFailure"
     reset_failure = "ResetFailure"
     under_voltage = "UnderVoltage"
     weak_signal = "WeakSignal"
 
-    # Soon to be deprecated enums
-    connectorLockFailure = "ConnectorLockFailure"
-    evCommunicationError = "EVCommunicationError"
-    groundFailure = "GroundFailure"
-    highTemperature = "HighTemperature"
-    internalError = "InternalError"
-    localListConflict = "LocalListConflict"
-    noError = "NoError"
-    otherError = "OtherError"
-    overCurrentFailure = "OverCurrentFailure"
-    overVoltage = "OverVoltage"
-    powerMeterFailure = "PowerMeterFailure"
-    powerSwitchFailure = "PowerSwitchFailure"
-    readerFailure = "ReaderFailure"
-    resetFailure = "ResetFailure"
-    underVoltage = "UnderVoltage"
-    weakSignal = "WeakSignal"
 
-
-class ChargePointStatus(str, Enum):
+class ChargePointStatus(StrEnum):
     """
     Status reported in StatusNotification.req. A status can be reported for
     the Charge Point main controller (connectorId = 0) or for a specific
     connector. Status for the Charge Point main controller is a subset of the
     enumeration: Available, Unavailable or Faulted.
 
     States considered Operative are: Available, Preparing, Charging,
@@ -172,34 +214,30 @@
     suspended_evse = "SuspendedEVSE"
     suspended_ev = "SuspendedEV"
     finishing = "Finishing"
     reserved = "Reserved"
     unavailable = "Unavailable"
     faulted = "Faulted"
 
-    # Soon to be deprecated enums
-    suspendedevse = "SuspendedEVSE"
-    suspendedev = "SuspendedEV"
-
 
-class ChargingProfileKindType(str, Enum):
+class ChargingProfileKindType(StrEnum):
     """
     "Absolute": Schedule periods are relative to a fixed point in time defined
                 in the schedule.
     "Recurring": Schedule restarts periodically at the first schedule period.
     "Relative": Schedule periods are relative to a situation- specific start
                 point(such as the start of a session)
     """
 
     absolute = "Absolute"
     recurring = "Recurring"
     relative = "Relative"
 
 
-class ChargingProfilePurposeType(str, Enum):
+class ChargingProfilePurposeType(StrEnum):
     """
     In load balancing scenarios, the Charge Point has one or more local
     charging profiles that limit the power or current to be shared by all
     connectors of the Charge Point. The Central System SHALL configure such
     a profile with ChargingProfilePurpose set to “ChargePointMaxProfile”.
     ChargePointMaxProfile can only be set at Charge Point ConnectorId 0.
 
@@ -231,114 +269,183 @@
     MUST be set to TxProfile.
     """
 
     charge_point_max_profile = "ChargePointMaxProfile"
     tx_default_profile = "TxDefaultProfile"
     tx_profile = "TxProfile"
 
-    # Soon to be deprecated enums
-    chargepointmaxprofile = "ChargePointMaxProfile"
-    txdefaultprofile = "TxDefaultProfile"
-    txprofile = "TxProfile"
 
-
-class ChargingProfileStatus(str, Enum):
+class ChargingProfileStatus(StrEnum):
     """
     Status returned in response to SetChargingProfile.req.
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
     not_supported = "NotSupported"
-    # Soon to be deprecated enums
-    notSupported = "NotSupported"
 
 
-class ChargingRateUnitType(str, Enum):
+class ChargingRateUnitType(StrEnum):
     """
     Unit in which a charging schedule is defined, as used in:
     GetCompositeSchedule.req and ChargingSchedule
     """
 
     watts = "W"
     amps = "A"
 
 
-class ClearCacheStatus(str, Enum):
+class CiStringType(int):
+    """
+    Generic used case insensitive string of X characters
+    """
+
+    ci_string_20 = 20
+    ci_string_25 = 25
+    ci_string_50 = 50
+    ci_string_255 = 255
+    ci_string_500 = 500
+
+
+class ClearCacheStatus(StrEnum):
     """
     Status returned in response to ClearCache.req.
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
 
 
-class ClearChargingProfileStatus(str, Enum):
+class ClearChargingProfileStatus(StrEnum):
     """
     Status returned in response to ClearChargingProfile.req.
     """
 
     accepted = "Accepted"
     unknown = "Unknown"
 
 
-class ConfigurationStatus(str, Enum):
+class ConfigurationStatus(StrEnum):
     """
     Status in ChangeConfiguration.conf.
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
     reboot_required = "RebootRequired"
     not_supported = "NotSupported"
 
-    # Soon to be deprecated enums
-    rebootRequired = "RebootRequired"
-    notSupported = "NotSupported"
+
+class ConfigurationKey(StrEnum):
+    """
+    Configuration Key Names.
+    """
+
+    # 9.1 Core Profile
+    allow_offline_tx_for_unknown_id = "AllowOfflineTxForUnknownId"
+    authorization_cache_enabled = "AuthorizationCacheEnabled"
+    authorize_remote_tx_requests = "AuthorizeRemoteTxRequests"
+    blink_repeat = "BlinkRepeat"
+    clock_aligned_data_interval = "ClockAlignedDataInterval"
+    connection_time_out = "ConnectionTimeOut"
+    connector_phase_rotation = "ConnectorPhaseRotation"
+    connector_phase_rotation_max_length = "ConnectorPhaseRotationMaxLength"
+    get_configuration_max_keys = "GetConfigurationMaxKeys"
+    heartbeat_interval = "HeartbeatInterval"
+    light_intensity = "LightIntensity"
+    local_authorize_offline = "LocalAuthorizeOffline"
+    local_pre_authorize = "LocalPreAuthorize"
+    max_energy_on_invalid_id = "MaxEnergyOnInvalidId"
+    meter_values_aligned_data = "MeterValuesAlignedData"
+    meter_values_aligned_data_max_length = "MeterValuesAlignedDataMaxLength"
+    meter_values_sampled_data = "MeterValuesSampledData"
+    meter_values_sampled_data_max_length = "MeterValuesSampledDataMaxLength"
+    meter_value_sample_interval = "MeterValueSampleInterval"
+    minimum_status_duration = "MinimumStatusDuration"
+    number_of_connectors = "NumberOfConnectors"
+    reset_retries = "ResetRetries"
+    stop_transaction_on_ev_side_disconnect = "StopTransactionOnEVSideDisconnect"
+    stop_transaction_on_invalid_id = "StopTransactionOnInvalidId"
+    stop_txn_aligned_data = "StopTxnAlignedData"
+    stop_txn_aligned_data_max_length = "StopTxnAlignedDataMaxLength"
+    stop_txn_sampled_data = "StopTxnSampledData"
+    stop_txn_sampled_data_max_length = "StopTxnSampledDataMaxLength"
+    supported_feature_profiles = "SupportedFeatureProfiles"
+    supported_feature_profiles_max_length = "SupportedFeatureProfilesMaxLength"
+    transaction_message_attempts = "TransactionMessageAttempts"
+    transaction_message_retry_interval = "TransactionMessageRetryInterval"
+    unlock_connector_on_ev_side_disconnect = "UnlockConnectorOnEVSideDisconnect"
+    web_socket_ping_interval = "WebSocketPingInterval"
+
+    # 9.2 Local Auth List Management Profile
+    local_auth_list_enabled = "LocalAuthListEnabled"
+    local_auth_list_max_length = "LocalAuthListMaxLength"
+    send_local_list_max_length = "SendLocalListMaxLength"
+
+    # 9.3 Reservation Profile
+    reserve_connector_zero_supported = "ReserveConnectorZeroSupported"
+
+    # 9.4 Smart Charging Profile
+    charge_profile_max_stack_level = "ChargeProfileMaxStackLevel"
+    charging_schedule_allowed_charging_rate_unit = (
+        "ChargingScheduleAllowedChargingRateUnit"
+    )
+    charging_schedule_max_periods = "ChargingScheduleMaxPeriods"
+    connector_switch_3to1_phase_supported = "ConnectorSwitch3to1PhaseSupported"
+    max_charging_profiles_installed = "MaxChargingProfilesInstalled"
+
+    # OCPP 1.6 ISO 15118 v10 added configuration keys
+    central_contract_validation_allowed = "CentralContractValidationAllowed"
+    certificate_signed_max_chain_size = "CertificateSignedMaxChainSize"
+    cert_signing_wait_minimum = "CertSigningWaitMinimum"
+    cert_signing_repeat_times = "CertSigningRepeatTimes"
+    certificate_store_max_length = "CertificateStoreMaxLength"
+    contract_validation_offline = "ContractValidationOffline"
+    iso_15118_pnc_enabled = "ISO15118PnCEnabled"
+
+    # OCPP security whitepaper added configuration keys
+    additional_root_certificate_check = "AdditionalRootCertificateCheck"
+    authorization_key = "AuthorizationKey"
+    cpo_name = "CpoName"
+    security_profile = "SecurityProfile"
 
 
-class DataTransferStatus(str, Enum):
+class DataTransferStatus(StrEnum):
     """
     Status in DataTransfer.conf.
     """
+
     accepted = "Accepted"
     rejected = "Rejected"
     unknown_message_id = "UnknownMessageId"
     unknown_vendor_id = "UnknownVendorId"
 
-    # Soon to be deprecated enums
-    unknownMessageId = "UnknownMessageId"
-    unknownVendorId = "UnknownVendorId"
-
 
-class DeleteCertificateStatus(str, Enum):
+class DeleteCertificateStatus(StrEnum):
     """
     DeleteCertificateStatusEnumType is used by: DeleteCertificate.conf
     """
 
     accepted = "Accepted"
     failed = "Failed"
     not_found = "NotFound"
 
 
-class DiagnosticsStatus(str, Enum):
+class DiagnosticsStatus(StrEnum):
     """
     Status in DiagnosticsStatusNotification.req.
     """
 
     idle = "Idle"
     uploaded = "Uploaded"
     upload_failed = "UploadFailed"
     uploading = "Uploading"
 
-    # Soon to be deprecated enums
-    uploadFailed = "UploadFailed"
 
-
-class FirmwareStatus(str, Enum):
+class FirmwareStatus(StrEnum):
     """
     Status of a firmware download as reported in FirmwareStatusNotification.req
     """
 
     # Common for:
     # FirmwareStatusNotification.req and SignedFirmwareStatusNotification.req
     downloaded = "Downloaded"
@@ -354,90 +461,86 @@
     download_paused = "DownloadPaused"
     install_rebooting = "InstallRebooting"
     install_scheduled = "InstallScheduled"
     install_verification_failed = "InstallVerificationFailed"
     invalid_signature = "InvalidSignature"
     signature_verified = "SignatureVerified"
 
-    # Soon to be deprecated enums
-    downloadFailed = "DownloadFailed"
-    installationFailed = "InstallationFailed"
-
 
-class GenericStatus(str, Enum):
+class GenericStatus(StrEnum):
     """
     Generic message response status
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
 
 
-class GetCompositeScheduleStatus(str, Enum):
+class GetCompositeScheduleStatus(StrEnum):
     """
     Status returned in response to GetCompositeSchedule.req
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
 
 
-class GetInstalledCertificateStatus(str, Enum):
+class GetInstalledCertificateStatus(StrEnum):
     """
     GetInstalledCertificateStatusEnumType is used by:
     GetInstalledCertificateIds.conf
     """
 
     accepted = "Accepted"
     not_found = "NotFound"
 
 
-class HashAlgorithm(str, Enum):
+class HashAlgorithm(StrEnum):
     """
     HashAlgorithmEnumType is used by: CertificateHashDataType
     """
 
     sha256 = "SHA256"
     sha384 = "SHA384"
     sha512 = "SHA512"
 
 
-class Location(str, Enum):
+class Location(StrEnum):
     """
     Allowable values of the optional "location" field of a value element in
     SampledValue.
     """
 
     inlet = "Inlet"
     outlet = "Outlet"
     body = "Body"
     cable = "Cable"
     ev = "EV"
 
 
-class Log(str, Enum):
+class Log(StrEnum):
     """
     LogEnumType is used by GetLog.req
     """
 
     diagnostics_log = "DiagnosticsLog"
     security_log = "SecurityLog"
 
 
-class LogStatus(str, Enum):
+class LogStatus(StrEnum):
     """
     LogStatusEnumType is used by: GetLog.conf
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
     accepted_canceled = "AcceptedCanceled"
 
 
-class Measurand(str, Enum):
+class Measurand(StrEnum):
     """
     Allowable values of the optional "measurand" field of a Value element, as
     used in MeterValues.req and StopTransaction.req messages. Default value of
     "measurand" is always "Energy.Active.Import.Register"
     """
 
     current_export = "Current.Export"
@@ -459,35 +562,16 @@
     power_reactive_export = "Power.Reactive.Export"
     power_reactive_import = "Power.Reactive.Import"
     rpm = "RPM"
     soc = "SoC"
     temperature = "Temperature"
     voltage = "Voltage"
 
-    # Soon to be deprecated enums
-    currentExport = "Current.Export"
-    currentImport = "Current.Import"
-    currentOffered = "Current.Offered"
-    energyActiveExportRegister = "Energy.Active.Export.Register"
-    energyActiveImportRegister = "Energy.Active.Import.Register"
-    energyReactiveExportRegister = "Energy.Reactive.Export.Register"
-    energyReactiveImportRegister = "Energy.Reactive.Import.Register"
-    energyActiveExportInterval = "Energy.Active.Export.Interval"
-    energyActiveImportInterval = "Energy.Active.Import.Interval"
-    energyReactiveExportInterval = "Energy.Reactive.Export.Interval"
-    energyReactiveImportInterval = "Energy.Reactive.Import.Interval"
-    powerActiveExport = "Power.Active.Export"
-    powerActiveImport = "Power.Active.Import"
-    powerFactor = "Power.Factor"
-    powerOffered = "Power.Offered"
-    powerReactiveExport = "Power.Reactive.Export"
-    powerReactiveImport = "Power.Reactive.Import"
 
-
-class MessageTrigger(str, Enum):
+class MessageTrigger(StrEnum):
     """
     Type of request to be triggered in a TriggerMessage.req
     """
 
     # Common for TriggerMessage.req and ExtendedTriggerMessage.req
     boot_notification = "BootNotification"
     firmware_status_notification = "FirmwareStatusNotification"
@@ -498,23 +582,16 @@
     # Only for TriggerMessage.req
     diagnostics_status_notification = "DiagnosticsStatusNotification"
 
     # Only for ExtendedTriggerMessage.req
     log_status_notification = "LogStatusNotification"
     sign_charge_point_certificate = "SignChargePointCertificate"
 
-    # Soon to be deprecated enums
-    bootNotification = "BootNotification"
-    diagnosticsStatusNotification = "DiagnosticsStatusNotification"
-    firmwareStatusNotification = "FirmwareStatusNotification"
-    meterValues = "MeterValues"
-    statusNotification = "StatusNotification"
-
 
-class Phase(str, Enum):
+class Phase(StrEnum):
     """
     Phase as used in SampledValue. Phase specifies how a measured value is to
     be interpreted. Please note that not all values of Phase are applicable to
     all Measurands.
     """
 
     l1 = "L1"
@@ -524,47 +601,31 @@
     l1_n = "L1-N"
     l2_n = "L2-N"
     l3_n = "L3-N"
     l1_l2 = "L1-L2"
     l2_l3 = "L2-L3"
     l3_l1 = "L3-L1"
 
-    # Soon to be deprecated enums
-    l1n = "L1-N"
-    l2n = "L2-N"
-    l3n = "L3-N"
-    l1l2 = "L1-L2"
-    l2l3 = "L2-L3"
-    l3l1 = "L3-L1"
-
 
-class ReadingContext(str, Enum):
+class ReadingContext(StrEnum):
     """
     Values of the context field of a value in SampledValue.
     """
 
     interruption_begin = "Interruption.Begin"
     interruption_end = "Interruption.End"
     other = "Other"
     sample_clock = "Sample.Clock"
     sample_periodic = "Sample.Periodic"
     transaction_begin = "Transaction.Begin"
     transaction_end = "Transaction.End"
     trigger = "Trigger"
 
-    # Soon to be deprecated enums
-    interruptionBegin = "Interruption.Begin"
-    interruptionEnd = "Interruption.End"
-    sampleClock = "Sample.Clock"
-    samplePeriodic = "Sample.Periodic"
-    transactionBegin = "Transaction.Begin"
-    transactionEnd = "Transaction.End"
 
-
-class Reason(str, Enum):
+class Reason(StrEnum):
     """
     Reason for stopping a transaction in StopTransaction.req.
     """
 
     emergency_stop = "EmergencyStop"
     ev_disconnected = "EVDisconnected"
     hard_reset = "HardReset"
@@ -573,99 +634,87 @@
     power_loss = "PowerLoss"
     reboot = "Reboot"
     remote = "Remote"
     soft_reset = "SoftReset"
     unlock_command = "UnlockCommand"
     de_authorized = "DeAuthorized"
 
-    # Soon to be deprecated enums
-    emergencyStop = "EmergencyStop"
-    evDisconnected = "EVDisconnected"
-    hardReset = "HardReset"
-    powerLoss = "PowerLoss"
-    softReset = "SoftReset"
-    unlockCommand = "UnlockCommand"
-    deAuthorized = "DeAuthorized"
-
 
-class RecurrencyKind(str, Enum):
+class RecurrencyKind(StrEnum):
     """
     "Daily": The schedule restarts at the beginning of the next day.
     "Weekly": The schedule restarts at the beginning of the next week
               (defined as Monday morning)
     """
 
     daily = "Daily"
     weekly = "Weekly"
 
 
-class RegistrationStatus(str, Enum):
+class RegistrationStatus(StrEnum):
     """
     Result of registration in response to BootNotification.req.
     """
 
     accepted = "Accepted"
     pending = "Pending"
     rejected = "Rejected"
 
 
-class RemoteStartStopStatus(str, Enum):
+class RemoteStartStopStatus(StrEnum):
     """
     The result of a RemoteStartTransaction.req or RemoteStopTransaction.req
     request.
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
 
 
-class ReservationStatus(str, Enum):
+class ReservationStatus(StrEnum):
     """
     Status in ReserveNow.conf.
     """
 
     accepted = "Accepted"
     faulted = "Faulted"
     occupied = "Occupied"
     rejected = "Rejected"
     unavailable = "Unavailable"
 
 
-class ResetStatus(str, Enum):
+class ResetStatus(StrEnum):
     """
     Result of Reset.req
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
 
 
-class ResetType(str, Enum):
+class ResetType(StrEnum):
     """
     Type of reset requested by Reset.req
     """
 
     hard = "Hard"
     soft = "Soft"
 
 
-class TriggerMessageStatus(str, Enum):
+class TriggerMessageStatus(StrEnum):
     """
     Status in TriggerMessage.conf.
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
     not_implemented = "NotImplemented"
 
-    # Soon to be deprecated enums
-    notImplemented = "NotImplemented"
 
-
-class UnitOfMeasure(str, Enum):
+class UnitOfMeasure(StrEnum):
     """
     Allowable values of the optional "unit" field of a Value element, as used
     in MeterValues.req and StopTransaction.req messages. Default value of
     "unit" is always "Wh".
     """
 
     wh = "Wh"
@@ -680,85 +729,73 @@
     kvar = "kvar"
     a = "A"
     v = "V"
     celsius = "Celsius"
     fahrenheit = "Fahrenheit"
     k = "K"
     percent = "Percent"
-    hertz = "Hertz"
 
 
-class UnlockStatus(str, Enum):
+class UnlockStatus(StrEnum):
     """
     Status in response to UnlockConnector.req.
     """
 
     unlocked = "Unlocked"
     unlock_failed = "UnlockFailed"
     not_supported = "NotSupported"
 
-    # Soon to be deprecated enums
-    unlockFailed = "UnlockFailed"
-    notSupported = "NotSupported"
-
 
-class UpdateFirmwareStatus(str, Enum):
+class UpdateFirmwareStatus(StrEnum):
     """
     UpdateFirmwareStatusEnumType is used by: SignedUpdateFirmware.conf
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
     accepted_canceled = "AcceptedCanceled"
     invalid_certificate = "InvalidCertificate"
     revoked_certificate = "RevokedCertificate"
 
 
-class UploadLogStatus(str, Enum):
+class UploadLogStatus(StrEnum):
     """
     UploadLogStatusEnumType is used by: LogStatusNotification.req
     """
 
     bad_message = "BadMessage"
     idle = "Idle"
     not_supported_operation = "NotSupportedOperation"
     permission_denied = "PermissionDenied"
     uploaded = "Uploaded"
     upload_failure = "UploadFailure"
     uploading = "Uploading"
 
 
-class UpdateStatus(str, Enum):
+class UpdateStatus(StrEnum):
     """
     Type of update for a SendLocalList.req.
     """
 
     accepted = "Accepted"
     failed = "Failed"
     not_supported = "NotSupported"
     version_mismatch = "VersionMismatch"
 
-    # Soon to be deprecated enums
-    notSupported = "NotSupported"
-    versionMismatch = "VersionMismatch"
 
-
-class UpdateType(str, Enum):
+class UpdateType(StrEnum):
     """
     Type of update for a SendLocalList.req.
     """
 
     differential = "Differential"
     full = "Full"
 
 
-class ValueFormat(str, Enum):
+class ValueFormat(StrEnum):
     """
     Format that specifies how the value element in SampledValue is to be
     interpreted.
     """
 
     raw = "Raw"
     signed_data = "SignedData"
-
-    # Soon to be deprecated enums
-    signedData = "SignedData"
```

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/AuthorizeResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/AuthorizeResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/BootNotification.json` & `ocpp-1.0.0/ocpp/v16/schemas/BootNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/BootNotificationResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/BootNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/ChangeAvailability.json` & `ocpp-1.0.0/ocpp/v16/schemas/ChangeAvailability.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/ClearChargingProfile.json` & `ocpp-1.0.0/ocpp/v16/schemas/ClearChargingProfile.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/DataTransferResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/DataTransferResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/DeleteCertificate.json` & `ocpp-1.0.0/ocpp/v16/schemas/DeleteCertificate.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/DeleteCertificateResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/DeleteCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/ExtendedTriggerMessage.json` & `ocpp-1.0.0/ocpp/v16/schemas/ExtendedTriggerMessage.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/FirmwareStatusNotification.json` & `ocpp-1.0.0/ocpp/v16/schemas/FirmwareStatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/GetCompositeSchedule.json` & `ocpp-1.0.0/ocpp/v16/schemas/GetCompositeSchedule.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/GetCompositeScheduleResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/GetCompositeScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/GetConfigurationResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/GetConfigurationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/GetDiagnostics.json` & `ocpp-1.0.0/ocpp/v16/schemas/GetDiagnostics.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/GetInstalledCertificateIds.json` & `ocpp-1.0.0/ocpp/v16/schemas/GetInstalledCertificateIds.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/GetLog.json` & `ocpp-1.0.0/ocpp/v16/schemas/GetLog.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/GetLogResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/GetLogResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/InstallCertificate.json` & `ocpp-1.0.0/ocpp/v16/schemas/InstallCertificate.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/InstallCertificateResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/InstallCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/LogStatusNotification.json` & `ocpp-1.0.0/ocpp/v16/schemas/LogStatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/MeterValues.json` & `ocpp-1.0.0/ocpp/v16/schemas/MeterValues.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/RemoteStartTransaction.json` & `ocpp-1.0.0/ocpp/v16/schemas/RemoteStartTransaction.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/ReserveNow.json` & `ocpp-1.0.0/ocpp/v16/schemas/ReserveNow.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/SendLocalList.json` & `ocpp-1.0.0/ocpp/v16/schemas/SendLocalList.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/SetChargingProfile.json` & `ocpp-1.0.0/ocpp/v16/schemas/SetChargingProfile.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/SignedFirmwareStatusNotification.json` & `ocpp-1.0.0/ocpp/v16/schemas/SignedFirmwareStatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/SignedUpdateFirmware.json` & `ocpp-1.0.0/ocpp/v16/schemas/SignedUpdateFirmware.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/StartTransaction.json` & `ocpp-1.0.0/ocpp/v16/schemas/StartTransaction.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/StartTransactionResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/StartTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/StatusNotification.json` & `ocpp-1.0.0/ocpp/v16/schemas/StatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/StopTransaction.json` & `ocpp-1.0.0/ocpp/v16/schemas/StopTransaction.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/StopTransactionResponse.json` & `ocpp-1.0.0/ocpp/v16/schemas/StopTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/TriggerMessage.json` & `ocpp-1.0.0/ocpp/v16/schemas/TriggerMessage.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v16/schemas/UpdateFirmware.json` & `ocpp-1.0.0/ocpp/v16/schemas/UpdateFirmware.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/AuthorizeRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/AuthorizeRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/AuthorizeResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/AuthorizeResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/BootNotificationRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/BootNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/BootNotificationResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/BootNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/CancelReservationRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/CancelReservationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/CancelReservationResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/CancelReservationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/CertificateSignedRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/CertificateSignedRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/CertificateSignedResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/CertificateSignedResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ChangeAvailabilityRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ChangeAvailabilityRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ChangeAvailabilityResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ChangeAvailabilityResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearCacheRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearCacheRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearCacheResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearCacheResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearChargingProfileRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearChargingProfileRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearChargingProfileResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearChargingProfileResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearDisplayMessageRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearDisplayMessageRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearDisplayMessageResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearDisplayMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearVariableMonitoringRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearVariableMonitoringRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearVariableMonitoringResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearVariableMonitoringResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearedChargingLimitRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearedChargingLimitRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ClearedChargingLimitResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ClearedChargingLimitResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/CostUpdatedRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/CostUpdatedRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/CostUpdatedResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/CostUpdatedResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/CustomerInformationRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/CustomerInformationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/CustomerInformationResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/CustomerInformationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/DataTransferRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/DataTransferRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/DataTransferResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/DataTransferResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/DeleteCertificateRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/DeleteCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/DeleteCertificateResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/DeleteCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/Get15118EVCertificateRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/Get15118EVCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/Get15118EVCertificateResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/Get15118EVCertificateResponse.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'properties'": "{'exiResponse': {'maxLength': 7500}}"}*

```diff
@@ -54,15 +54,15 @@
     },
     "properties": {
         "customData": {
             "$ref": "#/definitions/CustomDataType"
         },
         "exiResponse": {
             "description": "Raw CertificateInstallationRes response for the EV, Base64 encoded.\r\n",
-            "maxLength": 5600,
+            "maxLength": 7500,
             "type": "string"
         },
         "status": {
             "$ref": "#/definitions/Iso15118EVCertificateStatusEnumType"
         },
         "statusInfo": {
             "$ref": "#/definitions/StatusInfoType"
```

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetBaseReportRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetBaseReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetBaseReportResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetBaseReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetCertificateStatusRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetCertificateStatusRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetCertificateStatusResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetCertificateStatusResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetChargingProfilesRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetChargingProfilesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetChargingProfilesResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetChargingProfilesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetCompositeScheduleRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetCompositeScheduleRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetCompositeScheduleResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetCompositeScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetDisplayMessagesRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetDisplayMessagesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetDisplayMessagesResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetDisplayMessagesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetLocalListVersionRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetLocalListVersionRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetLocalListVersionResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetLocalListVersionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetLogRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetLogRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetLogResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetLogResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetMonitoringReportRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetMonitoringReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetMonitoringReportResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetMonitoringReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetReportRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetReportResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetTransactionStatusRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetTransactionStatusRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetTransactionStatusResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetTransactionStatusResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetVariablesRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetVariablesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/GetVariablesResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/GetVariablesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/HeartbeatRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/HeartbeatRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/HeartbeatResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/HeartbeatResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/InstallCertificateRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/InstallCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/InstallCertificateResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/InstallCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/LogStatusNotificationRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/LogStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/LogStatusNotificationResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/LogStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/MeterValuesRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/MeterValuesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/MeterValuesResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/MeterValuesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyChargingLimitRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyChargingLimitRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyChargingLimitResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyChargingLimitResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyCustomerInformationRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyCustomerInformationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyCustomerInformationResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyCustomerInformationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyEventRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyEventRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyEventResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyEventResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyMonitoringReportRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyMonitoringReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyMonitoringReportResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyMonitoringReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyReportRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/NotifyReportResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/NotifyReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/PublishFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/PublishFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ReportChargingProfilesRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ReportChargingProfilesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ReportChargingProfilesResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ReportChargingProfilesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/RequestStartTransactionRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/RequestStartTransactionRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/RequestStartTransactionResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/RequestStartTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/RequestStopTransactionRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/RequestStopTransactionRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/RequestStopTransactionResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/RequestStopTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ReservationStatusUpdateRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ReservationStatusUpdateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ReservationStatusUpdateResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ReservationStatusUpdateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ReserveNowRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ReserveNowRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ReserveNowResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ReserveNowResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ResetRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/ResetRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/ResetResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/ResetResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SecurityEventNotificationRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SecurityEventNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SecurityEventNotificationResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SecurityEventNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SendLocalListRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SendLocalListRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SendLocalListResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SendLocalListResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetChargingProfileRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetChargingProfileRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetChargingProfileResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetChargingProfileResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetDisplayMessageRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetDisplayMessageRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetDisplayMessageResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetDisplayMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringBaseRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetMonitoringBaseRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringBaseResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetMonitoringBaseResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringLevelRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetMonitoringLevelRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringLevelResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetMonitoringLevelResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetNetworkProfileRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetNetworkProfileRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetNetworkProfileResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetNetworkProfileResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetVariableMonitoringRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetVariableMonitoringRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetVariableMonitoringResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetVariableMonitoringResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetVariablesRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetVariablesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SetVariablesResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SetVariablesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SignCertificateRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/SignCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/SignCertificateResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/SignCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/StatusNotificationRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/StatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/StatusNotificationResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/StatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/TransactionEventRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/TransactionEventRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/TransactionEventResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/TransactionEventResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/TriggerMessageRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/TriggerMessageRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/TriggerMessageResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/TriggerMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/UnlockConnectorRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/UnlockConnectorRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/UnlockConnectorResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/UnlockConnectorResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/UnpublishFirmwareRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/UnpublishFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/UnpublishFirmwareResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/UnpublishFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/UpdateFirmwareRequest.json` & `ocpp-1.0.0/ocpp/v201/schemas/UpdateFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/ocpp/v201/schemas/UpdateFirmwareResponse.json` & `ocpp-1.0.0/ocpp/v201/schemas/UpdateFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.9.0/pyproject.toml` & `ocpp-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 [tool.poetry]
 name = "ocpp"
-version = "0.9.0"
+version = "1.0.0"
 description = "Python package implementing the JSON version of the Open Charge Point Protocol (OCPP)."
 authors = [
-	"Andre Duarte <andre.duarte@mobilityhouse.com>",
+	"André Duarte <andre15x@gmail.com>",
 	"Auke Willem Oosterhoff <aukewillem.oosterhoff@mobilityhouse.com>",
-	"Greg Lutostanski <greg.lutostanski@mobilityhouse.com>",
+	"Greg Lutostanski <greg.luto@gmail.com>",
+	"Jared Newell <jared.newell@mobilityhouse.com>",
 	"Jonathan Herrmann <jonathan.herrmann@mobilityhouse.com>",
-	"Laysa Uchoa <laysa.uchoadasilva@mobilityhouse.com>",
-	"Oz N Tiram, https://github.com/oz123",
-	"Patrick Roelke <patrick.roelke@mobilityhouse.com>",
+	"Laysa Uchoa <laysa.uchoa@gmail.com>",
+	"Oz N Tiram <oz.tiram@mobilityhouse.com>",
+	"Patrick Roelke <proelke@gmail.com>",
 	"Roger <roger.duran@mobilityhouse.com>",
 	"dx <dx@mobilityhouse.com>",
 	"Jan Vincke <jan.vincke@mobilityhouse.com>",
 ]
 repository = "https://github.com/mobilityhouse/ocpp"
 documentation = "https://ocpp.readthedocs.io/en/latest/"
 license = "MIT"
 readme = "README.rst"
 
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.6',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-
-# The dataclasses module is not in the stdlib in Python 3.6.
-dataclasses = { version = "^0.6", python = "~3.6" }
-jsonschema = "^3.0"
+python = "^3.8"
+jsonschema = "^4.4.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^4.5"
-pytest-asyncio = "^0.10.0"
-asynctest = "^0.13.0"
-freezegun = "^0.3.12"
-flake8 = "^3.7"
-pytest-cov = "^2.7"
-sphinx = "^2.1"
+# Starting from Python 3.8, asynctest is replaced with a unittest.mock.AsyncMock in standard library.
+pytest = "^7"
+pytest-asyncio = "^0.20.3"
+pytest-cov = "^4.0.0"
+sphinx = "^2.4.5"
+black = "^22"
+isort = "^5"
+flake8 = "^5"
+
+[tool.black]
+line-length = 88
+
+[tool.isort]
+profile = "black"
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["poetry>=1.1.11"]
 build-backend = "poetry.masonry.api"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ocpp-0.9.0/setup.py` & `ocpp-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,242 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ocpp
+Version: 1.0.0
+Summary: Python package implementing the JSON version of the Open Charge Point Protocol (OCPP).
+Home-page: https://github.com/mobilityhouse/ocpp
+License: MIT
+Author: André Duarte
+Author-email: andre15x@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
+Project-URL: Documentation, https://ocpp.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/mobilityhouse/ocpp
+Description-Content-Type: text/x-rst
 
-packages = \
-['ocpp', 'ocpp.v16', 'ocpp.v20', 'ocpp.v201']
+.. image:: https://github.com/mobilityhouse/ocpp/actions/workflows/pull-request.yml/badge.svg?style=svg
+   :target: https://github.com/mobilityhouse/ocpp/actions/workflows/pull-request.yml
 
-package_data = \
-{'': ['*'],
- 'ocpp.v16': ['schemas/*'],
- 'ocpp.v20': ['schemas/*'],
- 'ocpp.v201': ['schemas/*']}
-
-install_requires = \
-['jsonschema>=3.0,<4.0']
-
-extras_require = \
-{':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.6,<0.7']}
-
-setup_kwargs = {
-    'name': 'ocpp',
-    'version': '0.9.0',
-    'description': 'Python package implementing the JSON version of the Open Charge Point Protocol (OCPP).',
-    'long_description': '.. image:: https://circleci.com/gh/mobilityhouse/ocpp/tree/master.svg?style=svg\n   :target: https://circleci.com/gh/mobilityhouse/ocpp/tree/master\n\n.. image:: https://img.shields.io/pypi/pyversions/ocpp.svg\n   :target: https://pypi.org/project/ocpp/\n\n.. image:: https://img.shields.io/readthedocs/ocpp.svg\n   :target: https://ocpp.readthedocs.io/en/latest/\n\nOCPP\n----\n\nPython package implementing the JSON version of the Open Charge Point Protocol\n(OCPP). Currently OCPP 1.6 (errata v4), OCPP 2.0 and OCPP 2.0.1 (Final Version)\nare supported.\n\nYou can find the documentation on `rtd`_.\n\nInstallation\n------------\n\nYou can either the project install from Pypi:\n\n.. code-block:: bash\n\n   $ pip install ocpp\n\nOr clone the project and install it manually using:\n\n.. code-block:: bash\n\n   $ pip install .\n\nQuick start\n-----------\n\nBelow you can find examples on how to create a simple OCPP 2.0 central system as\nwell as an OCPP 2.0 charge point.\n\n.. note::\n\n   To run these examples the dependency websockets_ is required! Install it by running:\n\n   .. code-block:: bash\n\n      $ pip install websockets\n\nCentral system\n~~~~~~~~~~~~~~\n\nThe code snippet below creates a simple OCPP 2.0 central system which is able\nto handle BootNotification calls. You can find a detailed explanation of the\ncode in the `Central System documentation_`.\n\n\n.. code-block:: python\n\n    import asyncio\n    import logging\n    import websockets\n    from datetime import datetime\n\n    from ocpp.routing import on\n    from ocpp.v201 import ChargePoint as cp\n    from ocpp.v201 import call_result\n\n    logging.basicConfig(level=logging.INFO)\n\n\n    class ChargePoint(cp):\n        @on(\'BootNotification\')\n        async def on_boot_notification(self, charging_station, reason, **kwargs):\n            return call_result.BootNotificationPayload(\n                current_time=datetime.utcnow().isoformat(),\n                interval=10,\n                status=\'Accepted\'\n            )\n\n\n    async def on_connect(websocket, path):\n        """ For every new charge point that connects, create a ChargePoint\n        instance and start listening for messages.\n        """\n        try:\n            requested_protocols = websocket.request_headers[\n                \'Sec-WebSocket-Protocol\']\n        except KeyError:\n            logging.info("Client hasn\'t requested any Subprotocol. "\n                     "Closing Connection")\n        if websocket.subprotocol:\n            logging.info("Protocols Matched: %s", websocket.subprotocol)\n        else:\n            # In the websockets lib if no subprotocols are supported by the\n            # client and the server, it proceeds without a subprotocol,\n            # so we have to manually close the connection.\n            logging.warning(\'Protocols Mismatched | Expected Subprotocols: %s,\'\n                            \' but client supports  %s | Closing connection\',\n                            websocket.available_subprotocols,\n                            requested_protocols)\n            return await websocket.close()\n\n        charge_point_id = path.strip(\'/\')\n        cp = ChargePoint(charge_point_id, websocket)\n\n        await cp.start()\n\n\n    async def main():\n        server = await websockets.serve(\n            on_connect,\n            \'0.0.0.0\',\n            9000,\n            subprotocols=[\'ocpp2.0.1\']\n        )\n        logging.info("WebSocket Server Started")\n        await server.wait_closed()\n\n    if __name__ == \'__main__\':\n        asyncio.run(main())\n\nCharge point\n~~~~~~~~~~~~\n\n.. code-block:: python\n\n    import asyncio\n    import logging\n    import websockets\n\n    from ocpp.v201 import call\n    from ocpp.v201 import ChargePoint as cp\n\n    logging.basicConfig(level=logging.INFO)\n\n\n    class ChargePoint(cp):\n\n       async def send_boot_notification(self):\n           request = call.BootNotificationPayload(\n                   charging_station={\n                       \'model\': \'Wallbox XYZ\',\n                       \'vendor_name\': \'anewone\'\n                   },\n                   reason="PowerUp"\n           )\n           response = await self.call(request)\n\n           if response.status == \'Accepted\':\n               print("Connected to central system.")\n\n\n    async def main():\n       async with websockets.connect(\n           \'ws://localhost:9000/CP_1\',\n            subprotocols=[\'ocpp2.0.1\']\n       ) as ws:\n\n           cp = ChargePoint(\'CP_1\', ws)\n\n           await asyncio.gather(cp.start(), cp.send_boot_notification())\n\n\n    if __name__ == \'__main__\':\n       asyncio.run(main())\n\nDebugging\n---------\n\nPython\'s default log level is `logging.WARNING`. As result most of the logs\ngenerated by this package are discarded. To see the log output of this package\nlower the log level to `logging.DEBUG`.\n\n.. code-block:: python\n\n  import logging\n  logging.basicConfig(level=logging.DEBUG)\n\nHowever, this approach defines the log level for the complete logging system.\nIn other words: the log level of all dependencies is set to `logging.DEBUG`.\n\nTo lower the logs for this package only use the following code:\n\n.. code-block:: python\n\n  import logging\n  logging.getLogger(\'ocpp\').setLevel(level=logging.DEBUG)\n  logging.getLogger(\'ocpp\').addHandler(logging.StreamHandler())\n\nLicense\n-------\n\nExcept from the documents in `docs/v16` and `docs/v201` everything is licensed under MIT_.\n© `The Mobility House`_\n\nThe documents in `docs/v16` and `docs/v201` are licensed under Creative Commons\nAttribution-NoDerivatives 4.0 International Public License.\n\n.. _Central System documentation: https://ocpp.readthedocs.io/en/latest/central_system.html\n.. _MIT: https://github.com/mobilityhouse/ocpp/blob/master/LICENSE\n.. _rtd: https://ocpp.readthedocs.io/en/latest/index.html\n.. _The Mobility House: https://www.mobilityhouse.com/int_en/\n.. _websockets: https://pypi.org/project/websockets/\n',
-    'author': 'Andre Duarte',
-    'author_email': 'andre.duarte@mobilityhouse.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mobilityhouse/ocpp',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
-}
+.. image:: https://img.shields.io/pypi/pyversions/ocpp.svg
+   :target: https://pypi.org/project/ocpp/
 
+.. image:: https://img.shields.io/readthedocs/ocpp.svg
+   :target: https://ocpp.readthedocs.io/en/latest/
+
+OCPP
+----
+
+Python package implementing the JSON version of the Open Charge Point Protocol
+(OCPP). Currently OCPP 1.6 (errata v4), OCPP 2.0.1 (Edition 2 FINAL, 2022-12-15)
+are supported.
+
+You can find the documentation on `rtd`_.
+
+The purpose of this library is to provide the building blocks to construct a
+charging station/charge point and/or charging station management system
+(CSMS)/central system. The library does not provide a completed solution, as any
+implementation is specific for its intended use. The documents in this library
+should be inspected, as these documents provided guidance on how best to
+build a complete solution.
+
+Note: "OCPP 2.0.1 contains fixes for all the known issues, to date, not only
+the fixes to the messages. This version replaces OCPP 2.0. OCA advises
+implementers of OCPP to no longer implement OCPP 2.0 and only use version
+2.0.1 going forward."
+
+Installation
+------------
+
+You can either the project install from Pypi:
+
+.. code-block:: bash
+
+   $ pip install ocpp
+
+Or clone the project and install it manually using:
+
+.. code-block:: bash
+
+   $ pip install .
+
+Quick start
+-----------
+
+Below you can find examples on how to create a simple OCPP 1.6 or 2.0.1 Central
+System/CSMS as well as the respective OCPP 1.6 or 2.0.1
+Charging Station/Charge Point.
+
+.. note::
+
+   To run these examples the dependency websockets_ is required! Install it by running:
+
+   .. code-block:: bash
+
+      $ pip install websockets
+
+Charging Station Management System (CSMS) / Central System
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The code snippet below creates a simple OCPP 2.0.1 CSMS which
+is able to handle BootNotification calls. You can find a detailed explanation of the
+code in the `Central System documentation`_.
+
+
+.. code-block:: python
+
+    import asyncio
+    import logging
+    import websockets
+    from datetime import datetime
+
+    from ocpp.routing import on
+    from ocpp.v201 import ChargePoint as cp
+    from ocpp.v201 import call_result
+    from ocpp.v201.enums import RegistrationStatusType
+
+    logging.basicConfig(level=logging.INFO)
+
+
+    class ChargePoint(cp):
+        @on('BootNotification')
+        async def on_boot_notification(self, charging_station, reason, **kwargs):
+            return call_result.BootNotificationPayload(
+                current_time=datetime.utcnow().isoformat(),
+                interval=10,
+                status=RegistrationStatusType.accepted
+            )
+
+
+    async def on_connect(websocket, path):
+        """ For every new charge point that connects, create a ChargePoint
+        instance and start listening for messages.
+        """
+        try:
+            requested_protocols = websocket.request_headers[
+                'Sec-WebSocket-Protocol']
+        except KeyError:
+            logging.info("Client hasn't requested any Subprotocol. "
+                     "Closing Connection")
+            return await websocket.close()
+
+        if websocket.subprotocol:
+            logging.info("Protocols Matched: %s", websocket.subprotocol)
+        else:
+            # In the websockets lib if no subprotocols are supported by the
+            # client and the server, it proceeds without a subprotocol,
+            # so we have to manually close the connection.
+            logging.warning('Protocols Mismatched | Expected Subprotocols: %s,'
+                            ' but client supports  %s | Closing connection',
+                            websocket.available_subprotocols,
+                            requested_protocols)
+            return await websocket.close()
+
+        charge_point_id = path.strip('/')
+        cp = ChargePoint(charge_point_id, websocket)
+
+        await cp.start()
+
+
+    async def main():
+        server = await websockets.serve(
+            on_connect,
+            '0.0.0.0',
+            9000,
+            subprotocols=['ocpp2.0.1']
+        )
+        logging.info("WebSocket Server Started")
+        await server.wait_closed()
+
+    if __name__ == '__main__':
+        asyncio.run(main())
+
+Charging Station / Charge point
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    import asyncio
+
+    from ocpp.v201.enums import RegistrationStatusType
+    import logging
+    import websockets
+
+    from ocpp.v201 import call
+    from ocpp.v201 import ChargePoint as cp
+
+    logging.basicConfig(level=logging.INFO)
+
+
+    class ChargePoint(cp):
+
+        async def send_boot_notification(self):
+            request = call.BootNotificationPayload(
+                charging_station={
+                    'model': 'Wallbox XYZ',
+                    'vendor_name': 'anewone'
+                },
+                reason="PowerUp"
+            )
+            response = await self.call(request)
+
+            if response.status == RegistrationStatusType.accepted:
+                print("Connected to central system.")
+
+
+    async def main():
+        async with websockets.connect(
+                'ws://localhost:9000/CP_1',
+                subprotocols=['ocpp2.0.1']
+        ) as ws:
+            cp = ChargePoint('CP_1', ws)
+
+            await asyncio.gather(cp.start(), cp.send_boot_notification())
+
+
+    if __name__ == '__main__':
+        asyncio.run(main())
+
+Debugging
+---------
+
+Python's default log level is `logging.WARNING`. As result most of the logs
+generated by this package are discarded. To see the log output of this package
+lower the log level to `logging.DEBUG`.
+
+.. code-block:: python
+
+  import logging
+  logging.basicConfig(level=logging.DEBUG)
+
+However, this approach defines the log level for the complete logging system.
+In other words: the log level of all dependencies is set to `logging.DEBUG`.
+
+To lower the logs for this package only use the following code:
+
+.. code-block:: python
+
+  import logging
+  logging.getLogger('ocpp').setLevel(level=logging.DEBUG)
+  logging.getLogger('ocpp').addHandler(logging.StreamHandler())
+
+License
+-------
+
+Except from the documents in `docs/v16` and `docs/v201` everything is licensed under MIT_.
+© `The Mobility House`_
+
+The documents in `docs/v16` and `docs/v201` are licensed under Creative Commons
+Attribution-NoDerivatives 4.0 International Public License.
+
+.. _Central System documentation: https://ocpp.readthedocs.io/en/latest/central_system.html
+.. _MIT: https://github.com/mobilityhouse/ocpp/blob/master/LICENSE
+.. _rtd: https://ocpp.readthedocs.io/en/latest/index.html
+.. _The Mobility House: https://www.mobilityhouse.com/int_en/
+.. _websockets: https://pypi.org/project/websockets/
 
-setup(**setup_kwargs)
```

