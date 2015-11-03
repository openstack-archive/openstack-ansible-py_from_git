Example Index for role docs
===========================

This role is used for installing a python package from a git repository.
The role was build for the off chance that a special package will need to
be build from source without the use of an PyPi mirror or a links source.


Basic Role Example
^^^^^^^^^^^^^^^^^^

.. code-block:: yaml

    - role: "py_from_git"
      git_repo: "https://github.com/lxc/python2-lxc"
      git_dest: "/opt/lxc_python2_{{ git_install_branch|replace('/', '_') }}"
      git_install_branch: master
