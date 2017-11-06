Forked from https://github.com/numenta/manylinux for build
[PaddlePaddle](https://github.com/PaddlePaddle/Paddle) with manylinux1 support.

Since CUDA only support centos6 above docker images, use this to satisfy
CUDA and CUDNN requirements.


**IMPORTANT** Since this version of manylinux1_x86_64 is based on centos-6
(instead of centos-5), it is technically non-compliant with manylinux1 policy of
https://www.python.org/dev/peps/pep-0513/, which requires centos-5 system
libraries. However, as suggested in discussions
https://mail.python.org/pipermail/wheel-builders/2016-July/000175.html, the
wheels produced with the centos-6-based image should still be compatible with
many distros (except centos-5), and a future manylinux2 policy may indeed be
based on centos-6 as well.

See also [proof-of-concept nupic.bindings manylinux wheel build PR](https://github.com/numenta/nupic.core/pull/1001).
