#
# Copyright 2023 The Project Oak Authors
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#

load("@rules_java//java:defs.bzl", "java_test")

package(
    licenses = ["notice"],
)

java_test(
    name = "secure_service_test",
    srcs = ["SecureServiceImplTest.java"],
    test_class = "com.google.oak.example.SecureServiceImplTest",
    deps = [
        "//java/proto/example:secure_service_java_grpc",
        "//java/proto/example:secure_service_java_proto",
        "//java/src/main/java/com/google/oak/client",
        "//java/src/main/java/com/google/oak/crypto/hpke",
        "//java/src/main/java/com/google/oak/example",
        "//java/src/main/java/com/google/oak/remote_attestation:insecure_attestation_verifier",
        "//java/src/main/java/com/google/oak/server",
        "//java/src/main/java/com/google/oak/transport:grpc_streaming_transport",
        "//java/src/main/java/com/google/oak/util",
        "@com_google_protobuf//:protobuf_javalite",
        "@io_grpc_grpc_java//api",
        "@io_grpc_grpc_java//core:inprocess",
        "@org_assertj_assertj_core",
    ],
)
