|Build Status| |Coverage Status| |PyPI Version|

Flask-RBAC
==========

Adds RBAC support to Flask


Installation
------------

::

    $ pip install flask-rbac


Links
-----
- `Document <https://flask-rbac.readthedocs.org>`_
   补充：

   这是在Flask-RBAC的作者的基础上做了点扩展，因为不满足需求，需要根据个人的permission来判断权限而不是角色
   如果想要根据个人的permission来判断：
   ``rbac.set_user_permission(True)``
   同时User需要实现 ``get_permissions(self)`` 这个成员函数，返回permission list
   permission存的是request.endpoint

- `Issue Track <https://github.com/tiantaozhang/flask-rbac/issues>`_


Contributes
-----------

You can send a pull request on
`GitHub <https://github.com/tiantaozhang/flask-rbac/pulls>`_.


.. |Build Status| image:: https://travis-ci.org/shonenada/flask-rbac.png?branch=develop
   :target: https://travis-ci.org/shonenada/flask-rbac
.. |Coverage Status| image:: https://coveralls.io/repos/shonenada/flask-rbac/badge.png?branch=develop
   :target: https://coveralls.io/r/shonenada/flask-rbac
.. |PyPI Version| image:: https://img.shields.io/pypi/v/flask-rbac.svg?style=flat
   :target: https://pypi.python.org/pypi/flask-rbac
   :alt: PyPI Version
