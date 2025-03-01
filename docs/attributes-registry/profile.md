<!--- Hugo front matter used to generate the website version of this page:
--->

<!-- NOTE: THIS FILE IS AUTOGENERATED. DO NOT EDIT BY HAND. -->
<!-- see templates/registry/markdown/attribute_namespace.md.j2 -->

# Profile

## Profile Frame Attributes

Describes the origin of a single frame in a Profile.

| Attribute                                                                      | Type   | Description                                              | Examples  | Stability                                                        |
| ------------------------------------------------------------------------------ | ------ | -------------------------------------------------------- | --------- | ---------------------------------------------------------------- |
| <a id="profile-frame-type" href="#profile-frame-type">`profile.frame.type`</a> | string | Describes the interpreter or compiler of a single frame. | `cpython` | ![Experimental](https://img.shields.io/badge/-experimental-blue) |

`profile.frame.type` has the following list of well-known values. If one of them applies, then the respective value MUST be used; otherwise, a custom value MAY be used.

| Value     | Description                                                                                                                                                                                                                           | Stability                                                        |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| `cpython` | [Python](<https://wikipedia.org/wiki/Python_(programming_language)>)                                                                                                                                                                  | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `dotnet`  | [.NET](https://wikipedia.org/wiki/.NET)                                                                                                                                                                                               | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `jvm`     | [JVM](https://wikipedia.org/wiki/Java_virtual_machine)                                                                                                                                                                                | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `kernel`  | [Kernel](<https://wikipedia.org/wiki/Kernel_(operating_system)>)                                                                                                                                                                      | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `native`  | [C](<https://wikipedia.org/wiki/C_(programming_language)>), [C++](https://wikipedia.org/wiki/C%2B%2B), [Go](<https://wikipedia.org/wiki/Go_(programming_language)>), [Rust](<https://wikipedia.org/wiki/Rust_(programming_language)>) | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `perl`    | [Perl](https://wikipedia.org/wiki/Perl)                                                                                                                                                                                               | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `php`     | [PHP](https://wikipedia.org/wiki/PHP)                                                                                                                                                                                                 | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `ruby`    | [Ruby](<https://wikipedia.org/wiki/Ruby_(programming_language)>)                                                                                                                                                                      | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `v8js`    | [V8JS](<https://wikipedia.org/wiki/V8_(JavaScript_engine)>)                                                                                                                                                                           | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
