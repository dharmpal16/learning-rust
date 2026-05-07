
1. Create project in rust using cargo `cargo new my-project`
2. If you create rust project with ".gitignore" file then run `cargo new "foldername" --vcs=git`
3. To enter the project directory run this command `cd my-project`
4. build the project using `cargo build` command.
5. Run the `cargo run` to run the code in a very easy way.
6. If you forget command and you need quick help run `cargo new --help`
7. You can also use this command to create rust project using cargo `cargo init`
8. You can also use this command to run rust project using cargo `./target/debug/FOLDER_NAME_HERE`
9. Cargo also provides a command called `cargo check`. This command quickly checks your code to make sure it compiles but doesn’t produce an executable.

* Instead of saving the result of the build in the same directory as our code, Cargo stores it in the target/debug directory.
> An additional advantage of using Cargo is that the commands are the same no matter which operating system you’re working on. So, at this point, we’ll no longer provide specific instructions for Linux and macOS versus Windows.

### Building for Release
When your project is finally ready for release, you can use cargo build --release to compile it with optimizations. This command will create an executable in target/release instead of target/debug. The optimizations make your Rust code run faster, but turning them on lengthens the time it takes for your program to compile. This is why there are two different profiles: one for development, when you want to rebuild quickly and often, and another for building the final program you’ll give to a user that won’t be rebuilt repeatedly and that will run as fast as possible. If you’re benchmarking your code’s running time, be sure to run cargo build --release and benchmark with the executable in target/release.

