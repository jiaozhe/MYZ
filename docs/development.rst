开发
===============

.. contents:: 章节目录
   :depth: 2


制作文档
---------------
将源码 reST 文件，编译为 HTML 文档。

.. code-block:: shell

    $ cd MYZ/docs
    $ make html

**参考资料**

* 《reStructuredText入门》 <http://www.pythondoc.com/sphinx/rest.html>


打包发布
---------------
将项目打包为“源码（.tar.gz）包”和“Wheel包”，并发布到“PYPI（https://pypi.org）”站点。

.. code-block:: shell

    $ cd MYZ
    $ python setup.py sdist bdist_wheel
    $ twine upload dist/*
