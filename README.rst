cmdq
====

Simple command queue. Given a list of python callable, creates a thread pool to
unstack them concurrently.

Download
::::::::

git clone git://github.com/maisonsdumonde/cmdq.git
cd cmdq

Install in a virtualenv
:::::::::::::::::::::::

virtualenv .py-env
. .py-env/bin/activate
python setup.py develop

Install globally in the system
::::::::::::::::::::::::::::::

sudo python setup.py install

Syntax
::::::

cmdq config.cmdq

Config
::::::

For each command queue, create a .cmdq file using python syntax. The only
requirement is that it defines a cmdq local containing an iterable of the
python callables it needs to run. You can look at example.cmdq.

License
:::::::

Copyright (C) 2012 Maisons du Monde

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.