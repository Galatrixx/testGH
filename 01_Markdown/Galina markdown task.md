[//]: # (Galina Harjkova)

# Uzdevums 5
> Note: Data from repo https://github.com/hashicorp/terraform

Kādas izmaiņas tika veiktas iepriekšējās nedēļas laikā. Atrast vismaz divus veidus kā to izdarīt.
Command:
```sh
git log --since=7.days
```
OR use hardcoded dates like
```sh
git log --since='Aug 6 2023' --until='Aug 12 2023'
```
Results:
```sh
commit 3cce200d0eb6e1288d25110b4e029d762afe94e2 (HEAD -> main, origin/main, origin/HEAD)
Author: Liam Cervante <liam.cervante@hashicorp.com>
Date:   Wed Aug 9 15:21:31 2023 +0200

    Fix root cause of race condition in testing framework tests

commit f1ca74f09fbec614d4c4a02d19cc9e640e14ed6b
Author: Liam Cervante <liam.cervante@hashicorp.com>
Date:   Wed Aug 9 15:47:01 2023 +0200

    Update JSON_UI_VERSION after test framework changes

commit f8b1fe47dd45fedc19b1ad99ca453130f5c63c2c
Author: Liam Cervante <liam.cervante@hashicorp.com>
Date:   Wed Aug 9 11:19:00 2023 +0200

    Make config errors more important during init operations (#33628)

    * make config errors more important during init operations

    * address comments

commit e26d07dda41a74a009b1b750471395bf8773601c
Merge: 53431a245f ea1144995f
Author: James Bardin <j.bardin@gmail.com>
Date:   Tue Aug 8 12:40:57 2023 -0400

    Merge pull request #33634 from hashicorp/jbardin/init-from-module-warnings
    
```
Atrast commit kurus veica autors - “Laura Pacilio”
```sh
git log --author='Laura Pacilio'
```
Results:
```sh
commit 1ce0b91e67417ce0847f9fdac282145a9a881985
Merge: c1633436b8 97f9cb1645
Author: Laura Pacilio <83350965+laurapacilio@users.noreply.github.com>
Date:   Tue Nov 29 15:09:21 2022 -0500

    Merge pull request #32020 from hashicorp/fix-future-lang-2

    Remove future-facing language from docs (WIP)

commit 97f9cb16450869e0e64c45c28f1e5360cc39f446 (origin/fix-future-lang-2)
Author: Laura Pacilio <83350965+laurapacilio@users.noreply.github.com>
Date:   Tue Nov 29 15:00:36 2022 -0500

    Remove unnecessary explanation

commit a76b634f82b6a6f4d6df7f6829163b6c7ffd1812
Author: Laura Pacilio <83350965+laurapacilio@users.noreply.github.com>
Date:   Tue Nov 29 14:56:58 2022 -0500

    Update website/docs/internals/json-format.mdx

commit 0227952ace0e4dbf933578d0c483add3d19f35d5
Merge: 8664c9c1f8 a32648aa53
Author: Laura Pacilio <83350965+laurapacilio@users.noreply.github.com>
Date:   Wed Nov 9 11:08:58 2022 -0500

    Merge pull request #31274 from irab/patch-1

    Additional note on usage of single quotes for for_each resources
```

Atrast vai Laura ir veikusi commit pagājušā gada septembrī?
```sh
git log --after="2022-09-01" --before="2022-09-30" --author='Laura Pacilio'
```
Results
```sh
Yes, there are commits
```
Vai Laura ir veikusi commit vakar?
```sh
git log --since=yesterday.midnight --author='Laura Pacilio'
```
Results
```sh
No, no commits
```
