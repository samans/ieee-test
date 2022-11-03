# ieee-test

This is a test of an environment.

samans is the owner of this repository

samans-ncc75567 has a clone of this on their local pc

The idea is to have something like this "ieee-test" repository for use by IEEE 802.1 Yang editors.
The IEEE 802.1 Yang editors would not need to fork or clone the IETF's YangModels/Yang.
IEEE 802.1 YANGsters could appoint a few people to merge the changes from the IEEE's repository to the IETF's repository.

In the tutorial powerpoint:
- Step 1 (sync local)
    - git checkout main
    - git pull
- Step 2 (make local changes)
    - git checkout -b foobar-04
    - (make some changes to a file)
    - git status
    - git commit -am "some commit message"
- Step 3 (resync) (note:  in the tutorial I introduced a change to the origin main, to illustrate what happens)
    - git checkout main
    - git pull
    - git checkout foobar-04
    - git merge main foobar-04 (this is the command that would show conflicts that need to be resolved -- none in this example)
 - Step 4 (push branch to origin)
    - git checkout foobar-04
    - git push origin foobar-04
 - Step 5 (pull request to suggest your branch to origin)
    - This is done at https://github.com/samans/ieee-test while logged in as samans-ncc75567 (or whatever the editors github id is)
 - Step 6
    - The "yang leader" logs in to https://github.com/samans/ieee-test (in this example as samans) and clicks the "Merge pull request" button
    - The branch can be deleted after it is successfully merged
 - Step 7
    - The "yang leader" then follows the existing process to do a pull request of the changes to the IETF's YangModels/yang repository
