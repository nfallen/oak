#
# Copyright 2022 The Project Oak Authors
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

package(
    default_visibility = ["//visibility:public"],
    licenses = ["notice"],
)

filegroup(
    name = "srcs",
    srcs = glob(
        ["tensorflow/lite/**/*.cc"],
        exclude = [
            "tensorflow/lite/micro/debug_log.cc",
        ],
    ),
)

filegroup(
    name = "hdrs",
    srcs = glob(["tensorflow/lite/**/*.h"]),
)

filegroup(
    name = "generate_cc_arrays",
    srcs = ["tensorflow/lite/micro/tools/generate_cc_arrays.py"],
)
