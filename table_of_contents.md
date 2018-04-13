
# Google Test Documentation Table Of Contents#

--- Basic README.md ---
Location: googletest/README.md
Sections: -Features
          -Platforms
          -Who Is Using Google Test?
          -Related Open Source Projects
          -Requirements
            -Linux Requirements
            -Windows Requirements
            -Cygwin Requirements
            -Mac OS X Requirements
          -Contributing Change


--- Primer.md ---
Location: googletest/googletest/docs/Primer.md
Sections: -Introduction: Why Google C++ Testing Framework?
          -Beware of the nomenclature
          -Setting up a New Test Project
          -Basic Concepts
          -Assertions
          -Basic Assertions
          -Binary Comparison
          -String Comparison
          -Simple Tests
          -Test Fixtures: Using the Same Data Configuration for Multiple Tests
          -Invoking the Tests
          -Writing the main() Function
          -Important note for Visual C++ users
          -Where to Go from Here
          -Known Limitations


--- Google Mock's README.md ---
Location: googletest/googlemock/README.md
Sections: -Google Mock
            -Overview
            -Features
          -Getting Started
            -Using Google Mock Without Google Test
            -Requirements for End Users
              -Linux Requirements
              -Windows Requirements
              -Mac OS X Requirements
            -Requirements for Contributors
            -Building Google Mock
              -Using CMake
              -Preparing to Build (Unix only)
            -Windows
            -Tweaking Google Mock
            -Choosing a TR1 Tuple Library
            -As a Shared Library (DLL)
            -Tweaking Google Mock
            -Upgrading from an Earlier Version
              -Upgrading from 1.1.0 or Earlier
              -Upgrading from 1.4.0 or Earlier


--- Google Test README.md ---
Location: googletest/googletest/README.md            
Sections: -Generic Build Instructions
            -Setup
            -Build
          -Using CMake
            -Standalone CMake Project
            -Incorporating Into An Existing CMake Project
            -Visual Studio Dynamic vs Static Runtimes
          -Legacy Build Scripts
          -Tweaking Google Test
          -Choosing a TR1 Tuple Library
          -Multi-threaded Tests
          -As a Shared Library (DLL)
          -Avoiding Macro Name Clashes


--- Contributing CONTRIBUTING.md ---
Location: googletest/CONTRIBUTING.md
Sections: -How to become a contributor and submit your own code
            -Contributor License Agreements
            -Contributing A Patch
            -The Google Test and Google Mock Communities
              -Please Be Friendly
            -Style
            -Requirements for Contributors
            -Developing Google Test
              -Testing Google Test Itself
              -Regenerating Source Files
            -Developing Google Mock
              -Testing Google Mock Itself


--- Advanced Google Test Guide AdvancedGuide.md ---
Location: googletest/googletest/docs/AdvancedGuide.md
Sections: -More Assertions
            -Explicit Success and Failure
            -Exception Assertions
            -Predicate Assertions for Better Error Messages
              -Using an Existing Boolean Function
              -Using a Function That Returns an AssertionResult
              -Using a Predicate-Formatter
            -Floating-Point Comparison
              -Floating Point Macros
              -Floating-Point Predicate-Format Functions
            -Windows HRESULT assertions
            -Type Assertions
            -Assertion Placement
          -Teaching Google Test How to Print Your Values
          -Death Tests
            -How to Write a Death Test
            -Regular Expression Syntax
            -How It Works
            -Death Tests And Threads
            -Death Test Styles
            -Caveats
          -Using Assertions in Sub-routines
            -Adding Traces to Assertions
            -Propagating Fatal Failures
              -Asserting on Subroutines with an exception
              -Asserting on Subroutines
              -Checking for Failures in the Current Test
          -Logging Additional Information
          -Sharing Resources Between Tests in the Same Test Case
          -Global Set-Up and Tear-Down
          -Value Parameterized Tests
            -How to Write Value-Parameterized Tests
            -Creating Value-Parameterized Abstract Tests
          -Typed Tests
          -Type-Parameterized Tests
          -Testing Private Code
            -Static Functions
            -Private Class Members
          -Catching Failures
          -Getting the Current Test's Name
          -Extending Google Test by Handling Test Events
            -Defining Event Listeners
            -Using Event Listeners
            -Generating Failures in Listeners
          -Running Test Programs: Advanced Options
            -Selecting Tests
              -Listing Test Names
              -Running a Subset of the Tests
              -Temporarily Disabling Tests
              -Temporarily Enabling Disabled Tests
            -Repeating the Tests
            -Shuffling the Tests
            -Controlling Test Output
              -Colored Terminal Output
              -Suppressing the Elapsed Time
              -Suppressing UTF-8 Text Output
              -Generating an XML Report
              -Generating an JSON Report {#JsonReport}
            -Controlling How Failures Are Reported
              -Turning Assertion Failures into Break-Points
              -Disabling Catching Test-Thrown Exceptions
              -Letting Another Testing Framework Drive
            =Distributing Test Functions to Multiple Machines
          -Fusing Google Test Source Files
          -Where to Go from Here


--- Frequently Asked Questions FAQ.md ---
Location: googletest/googletest/docs/FAQ.md
Sections: -Why should I use Google Test instead of my favorite C++ testing framework?
          -I'm getting warnings when compiling Google Test. Would you fix them?
          -Why should not test case names and test names contain underscore?
          -Why is it not recommended to install a pre-compiled copy of Google Test (for example, into /usr/local)?
          -How do I generate 64-bit binaries on Windows (using Visual Studio 2008)?
          -Can I use Google Test on MinGW?
          -Why does Google Test support EXPECT_EQ(NULL, ptr) and ASSERT_EQ(NULL, ptr) but not EXPECT_NE(NULL, ptr) and ASSERT_NE(NULL, ptr)?
          -Does Google Test support running tests in parallel?
          -Why don't Google Test run the tests in different threads to speed things up?
          -Why aren't Google Test assertions implemented using exceptions?
          -Why do we use two different macros for tests with and without fixtures?
          -Why don't we use structs as test fixtures?
          -Why are death tests implemented as assertions instead of using a test runner?
          -My death test modifies some state, but the change seems lost after the death test finishes. Why?
          -The compiler complains about "undefined references" to some static const member variables, but I did define them in the class body. What's wrong?
          -I have an interface that has several implementations. Can I write a set of tests once and repeat them over all the implementations?
          -Can I derive a test fixture from another?
          -My compiler complains "void value not ignored as it ought to be." What does this mean?
          -My death test hangs (or seg-faults). How do I fix it?
          -Should I use the constructor/destructor of the test fixture or the set-up/tear-down function?
          -The compiler complains "no matching function to call" when I use ASSERT_PREDn. How do I fix it?
          -My compiler complains about "ignoring return value" when I call RUN_ALL_TESTS(). Why?
          -My compiler complains that a constructor (or destructor) cannot return a value. What's going on?
          -My set-up function is not called. Why?
          -How do I jump to the line of a failure in Emacs directly?
          -I have several test cases which share the same test fixture logic, do I have to define a new test fixture class for each of them? This seems pretty tedious.
          -The Google Test output is buried in a whole bunch of log messages. What do I do?
          -Why should I prefer test fixtures over global variables?
          -How do I test private class members without writing FRIEND_TEST()s?
          -How do I test private class static members without writing FRIEND_TEST()s?
          -I would like to run a test several times with different parameters. Do I need to write several similar copies of it?
          -How do I test a file that defines main()?
          -What can the statement argument in ASSERT_DEATH() be?
          -What syntax does the regular expression in ASSERT_DEATH use?
          -I have a fixture class Foo, but TEST_F(Foo, Bar) gives me error "no matching function for call to Foo::Foo()". Why?
          -Why does ASSERT_DEATH complain about previous threads that were already joined?
          -Why does Google Test require the entire test case, instead of individual tests, to be named FOODeathTest when it uses ASSERT_DEATH?
          -But I don't like calling my entire test case FOODeathTest when it contains both death tests and non-death tests. What do I do?
          -The compiler complains about "no match for 'operator<<'" when I use an assertion. What gives?
          -How do I suppress the memory leak messages on Windows?
          -I am building my project with Google Test in Visual Studio and all I'm getting is a bunch of linker errors (or warnings). Help!
          -I put my tests in a library and Google Test doesn't run them. What's happening?
          -I want to use Google Test with Visual Studio but don't know where to start.
          -I am seeing compile errors mentioning std::type_traits when I try to use Google Test on Solaris.
          -How can my code detect if it is running in a test?
          -Google Test defines a macro that clashes with one defined by another library. How do I deal with that?
          -Is it OK if I have two separate TEST(Foo, Bar) test methods defined in different namespaces?
          -How do I build Google Testing Framework with Xcode 4?
          -How do I easily discover the flags needed for GoogleTest?
          -My question is not covered in your FAQ!
          
