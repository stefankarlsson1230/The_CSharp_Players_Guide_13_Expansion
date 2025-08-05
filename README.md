# The C# Player's Guide - C# 13 Expansion


.NET 9 Projects
Read after Level 2: Getting an IDE
    1. Version Validator – Create a tool that checks if .NET 9 is available on the system.
    2. Target Updater – Allow the user to pick a project and programmatically change the target framework to .NET 9.
    3. Feature Flag Toggle – Use preprocessor directives to enable or disable features based on version checks.
    4. Version-Specific Code Tester – Include a class that behaves differently in .NET 6, .NET 8, and .NET 9.
    5. Multi-Framework Library – Create a multi-targeted class library that compiles under both .NET 8 and .NET 9.

The Escape Character (\e)
Read after Level 8: Console 2.0
    1. Color Demo Console – Display text in a full RGB color (e.g., vibrant orange) using \e[38;2;R;G;Bm.
    2. Named Color Set – Create reusable string variables for six colors and use them to style different lines of output.
    3. Escape Reset Test – Combine text with color and reset commands (\e[39m, \e[49m) to isolate color effects.
    4. Dynamic Color Picker – Let users input RGB values and generate corresponding escape sequences to color text.
    5. ANSI Showcase – Cycle through underline, bold, italics, etc., using ANSI escape codes and document which work on your console.

Challenge: The Six Staffs of Elegedd
    1. Staff Renderer – Print 6 vertical lines of ---* representing each staff.
    2. Color Encoder – Apply a unique RGB color to each line using ANSI codes and escape sequences.
    3. Color Definitions – Define each color (RGB triplet) in named variables, then use $"{color}..." in output.
    4. Color Reset Logic – Add \e[39m to reset color after each line.
    5. Compatibility Test – Detect if ANSI codes are supported in current terminal and switch to ConsoleColor as fallback.

Challenge: Finding the Henges
Read after Level 17: Tuples
    1. Enum Builder – Create a Henge enum listing six henge names.
    2. GetInformation Method – Return (X, Y, DisplayText) tuple using a switch expression.
    3. Display with Positioning – Set cursor with Console.SetCursorPosition(x, y) and display each henge using Console.Write().
    4. Color String Builder – Add RGB coloring to the displayed character using ANSI escape strings.
    5. Map Triangulation – Arrange output to form a triangle when viewing in the console.

Challenge: Amaranth and Jasmine
Read after Level 23: Object-Oriented Design
    1. Location Class – Implement a class with int X and int Y properties.
    2. Color Class – Use get-only properties and constructor for RGB values; add GetColorText() method returning escape string.
    3. Henge Class – Add fields for location, color, and representation; implement Display() using cursor positioning and color.
    4. Main Program Logic – Create two Henge instances using Location, Color, and char values, and display both.
    5. Separation of Concerns – Refactor Display() logic into a helper method reused for both henges.

Challenge: The Henges of Elegedd
Read after Level 23: Object-Oriented Design
    1. Crate Class – Add a Location field, IsIntact property, constructor, and Display() method.
    2. Henge Array Setup – Build an array of 6 Henge objects using known data (position, char, RGB).
    3. Crate Array Setup – Create 4 Crate instances and store in array.
    4. Controller Logic – Implement keyboard controls for movement (arrow keys) and selection (D1–D6).
    5. Interaction Logic – On Spacebar, if henge and crate share location, mark IsIntact = false and remove visually.

More Flexible params
Read after Level 34: Methods Revisited
    1. List-Based Averager – Rewrite Average() to take params List<int> instead of array.
    2. Flexible Print – Pass either an array or a List<string> into the same method signature.
    3. Generic Collector – Accept any collection type (array, List<T>, IEnumerable<T>) and process it uniformly.
    4. Command Logger – Create a command interface that logs any number of command steps using flexible params.
    5. Hybrid Params Demo – Accept optional header string followed by params IEnumerable<T> and format accordingly.

System.Threading.Lock
Read after Level 43: Threads
    1. Lock Conversion – Replace old object lock fields with System.Threading.Lock.
    2. Safe Counter – Create a thread-safe counter that increments and reads values using lock (_lock).
    3. Race Condition Demo – Simulate a race condition using object, then fix it using Lock.
    4. Performance Comparison – Benchmark a synchronized counter using Monitor vs Lock.
    5. Multi-Lock Coordination – Use two Lock objects to protect two fields and avoid deadlocks during concurrent access.


