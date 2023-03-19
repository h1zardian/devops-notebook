---
id: 7x8bo0zs4f2z1nm948idpka
title: init containers
desc: ''
updated: 1678170039089
created: 1678169129099
---

- Init containers runs to completion and runs before the main container starts. These containers can contain certain utilities or custom code for the setup that is not present for the app container.

- These can also be used to delay the start of the main containers by having some precondition check; unless they are met, it will keep trying the init containers.
