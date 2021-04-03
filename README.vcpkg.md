branch vcpkg - WIP

# motivation
I'm not familiar with conan but like vcpkg.  I really like this template, but not quite ready to abandon vcpkg for conan.  Although Jason makes it very tempting.

# goals
- enable template to work with vcpkg without losing functionality

# potential goals
- compare vcpkg/conan, if I can get this to work equally well with either, makes comparing them possible.

# usage
This isn't yet as nice as conan so you'll have to install the vcpkg packages yourself. To find what you need
```
ls -Recurse CMakeLists.txt|Select-String find_package
```
And then install what is needed.

# known issues
CI not working with vcpkg.  Not sure how easy this will be to fix:
- maybe just install both in CI
- maybe just leverage conan in CI since it already works
