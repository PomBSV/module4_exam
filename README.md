# CAS-DAS UNIBE 2019-2020
## Module 5: GitHub repository, patch file, documentation techniques

### Maya Polanco

#### Oral examination


1. Git repository and patch file

![](images/fig1.png?raw=true)

Objective
Single change done in a branch, translate it to another branch

General idea
1. We have create 3 branches in our local repository 
Branch **branch_test_patch** I added next text at the end of version M3_randomforest.ipynb

"I added this text to set up a ppatch file ".
Branch **brach_where_i_want_to_copy** is just a version of the original  M3_randomforest.ipynb

2.Checkout the branch where the change we want to replicate has been done


command
```ruby
git format-patch brach_where_i_want_to_copy -o patches
puts markdown.to_html
```
To remember: 
```ruby
'branch_test_patch' where we have the change for first time
"brach_where_i_want_to_copy" branch where I want to apply the change
puts markdown.to_html
``` 
Command to create a patch file, where we write the name of the branch which is the branch where we want to apply the changes,"brach_where_i_want_to_copy" git is going to compare the 2 branches and we will get the differences in the patch file. Git will save the patch file in a directory on the project root calle 'patches'.




Last Update: 3.07.2020
