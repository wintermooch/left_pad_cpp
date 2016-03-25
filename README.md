# left_pad_cpp

Unopinionated C++ version of the popular left_pad

# Features

* In not_kik namespace. Makes it safer from future lawsuits.
* Two functions provided, as well as object oriented interface.
* Portable.
* Not written in JavaScript.

# Usage 

    std::cout << not_kik::LeftPad("foo", 5, '+') << std::endl;
    std::cout << not_kik::LeftPad("foo", -1, '+') << std::endl;

Outputs:
    ++foo
    foo

    std::string foo("foo");
    not_kik::LeftPad(5, '+', &foo);
    std::cout << foo << std::endl;
    foo = "foo";
    not_kik::LeftPad(-1, '+', &foo);
    std::cout << foo << std::endl;

Outputs:

    ++foo
    foo

    not_kik::LeftPadder plus_left_padder('+');
    std::cout << plus_left_padder.Pad("foo", 5) << std::endl;
    std::cout << plus_left_padder.Pad("foo", -2) << std::endl;

Outputs:

    ++foo
    foo

# Future work

* Python bindings.
* Better unit testing with gtest framework.

# Support

Please sponsor future developments of the left_pad_cpp library: 191vGngyDnpznFBNaWsKy5FySqwAWEhTBQ.

# License

Commercial license is available, in case you don't like the advertising BSD license.
