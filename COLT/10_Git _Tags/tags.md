## Tags

Git Tags are pointers that refer to particulars points in Git History. It is often used
to mark a version releases in Projects (v6.10, v6.15 etc).




## Type Of Tags

1. Light Weight Tags -> They are just a name/label attached to a commit

2. Annotated Tags -> Store Extra meta data




## Semantic Versioning
It is a rule / standard for naming software versions.

It always consist of 3 parts -> *Major Release . Minor Release . Minor Patch  
Ex : 4.5.8

*Major Release* (4) -> First part of Semantic Versioning is Major Release. It is a breaking change in software. No backward compatibility
When Major Release happens,  Minor Release Number and Path Release Number Reset to 0



*Minor Release* (5) ->  Second part of Semantic Versioning is Minor Release. It is a new feature added in software. But the Projects
is still backward compatible. No Breaking Changes. New Features is OPTIONAL. When Minor Release happens, Path Release Number Reset to 0



*Path Release* (8) -> Last part of Semantic Versioning is Path Release. It does not contain any new Features. Typically it is a bug fix.




## View Tags

git tag  -> It Showw all Tags

git tag -l ""  -> It Showw all Tags that match the Pattern "" ("" is a Wild Card). Ex : git tag -l "v*"



## Checking Out Tags

git checkout <tag name>

Checking Out Tags is checkout a particular commit



## Creating Light Weight 

git tag <tag name>

example : git tag v6.10

How To -> After Commenting the code we create Tag and push it to remote repository