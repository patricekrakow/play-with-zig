# Let's Play with Zig

I’m amazed that I only discovered [Zig](https://ziglang.org/) yesterday (June 18, 2026) while casually browsing YouTube: [
Zig 2026: No-AI Policy, $670K Foundation, Left GitHub & Why Zig Isn’t 1.0 - Andrew Kelley Explains](https://youtu.be/iqddnwKF8HQ?si=oFWxbz9o32wrIldH).

## Installing Zig

### Installing Zig on Windows

1\. Got to <https://ziglang.org/>.

2\. Click on the hamburger and click on the "Download" link, <https://ziglang.org/download/>.

3\. Then, for the section with the highest version number, just after the "master" one, click on "zig-x86_64-windows-0.16.0.zip" link, <https://ziglang.org/download/0.16.0/zig-x86_64-windows-0.16.0.zip>.

4\. Unzip the file `zig-x86_64-windows-0.16.0.zip` into the folder `C:\Users\{Username}\AppData\Local\Programs`, it will create the sub-folder `zig-x86_64-windows-0.16.0` in it.

> ***Note:*** You may have to create the sub-folder `Programs` within the folder `C:\Users\{Username}\AppData\Local`.

5\. Open a _Command Prompt_ and type the following command:

```text
rundll32 sysdm.cpl, EditEnvironmentVariables
```

It will open a "Environment Variables" window.

6\. Within the "User variables for {Username}" section, click on the "New..." button, type `ZIG_BIN` in the "Variable name" edit box, type `C:\Users\{Username}\AppData\Local\Programs\zig-x86_64-windows-0.16.0` in the "Variable value" edit box, and click on the "OK" button.

7\. Still within the "User variables for {Username}" section, scroll down to locate the `Path` variable, click on it, and click on the "Edit..." button, it will open a "Edit environment variable" dialog box.

8\. Click on the "New" button, type `%ZIG_BIN%`, and click on the OK button.

9\. Click on the "OK" button of the "Environment Variables" window.

10\. To verify the installtion, close your current _Command Prompt_, open a new one, and type the following commands:

```text
zig version
```

## References

* (n.d.). _Getting Started. Zig._ Retrieved June 18, 2026, from <https://ziglang.org/learn/getting-started/>
