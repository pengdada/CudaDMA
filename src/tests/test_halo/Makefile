#  Copyright 2010 NVIDIA Corporation
#
#  Licensed under the Apache License, Version 2.0 (the "License");
#  you may not use this file except in compliance with the License.
#  You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
#  Unless required by applicable law or agreed to in writing, software
#  distributed under the License is distributed on an "AS IS" BASIS,
#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#  See the License for the specific language governing permissions and
#  limitations under the License.

all: test_halo

test_halo: ../../../include/cudaDMA.h cudaDMA_test_halo.cu
	nvcc -I../../../include -o test_halo -O2 -arch=compute_20 -code=sm_20 cudaDMA_test_halo.cu 

clean:
	rm -f *.o test_halo
