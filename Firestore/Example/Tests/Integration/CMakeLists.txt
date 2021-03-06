# Copyright 2019 Google
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

if(APPLE)
  objc_test(
    firebase_firestore_objc_integration_test
    HOST firestore_example_app_macos
    SOURCES
      FSTSmokeTests.mm
      FSTDatastoreTests.mm
      FSTTransactionTests.mm
      API/FIRArrayTransformTests.mm
      API/FIRFieldsTests.mm
      API/FIRNumericTransformTests.mm
      API/FIRTypeTests.mm
      API/FIRCursorTests.mm
      API/FIRFirestoreSourceTests.mm
      API/FIRQueryTests.mm
      API/FIRValidationTests.mm
      API/FIRDatabaseTests.mm
      API/FIRListenerRegistrationTests.mm
      API/FIRServerTimestampTests.mm
      API/FIRWriteBatchTests.mm
    DEPENDS
      FirebaseFirestore
      firebase_firestore_objc_test_util
  )
endif(APPLE)
