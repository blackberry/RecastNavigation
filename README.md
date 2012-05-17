# RecastNavigation v1.4

The _**RecastNavigation**_ repository holds the sources for the Recast Navigation, navigation-mesh construction toolset for Games. The Detour, DetourCrowd and Recast libraries have been additionally ported to run with the BlackBerry Native SDK for BlackBerry Tablet OS and BlackBerry 10 OS.

**Repository Committers** 

* [Sean Paul Taylor](https://github.com/seanpaultaylor)

## Building for BlackBerry

Building from Command-line:

    - cd [bbndk]                    where [bbndk] is where the QNX NDK was installed (i.e. C:\bbndk)
    - bbndk-env.bat                 on Windows or bbndk-env.sh on MacOSX or Linux
    - cd [RecastNavigation]/qnx		where [RecastNavigation] is the directory where RecastNavigation was extracted to
    - make

Following this, the relevant static libraries should reside in the following subdirectories:

    libDetour: 
        [RecastNavigation]/qnx/Detour/arm/a.le.v7           (ARM release)
        [RecastNavigation]/qnx/Detour/arm/a.le.v7.g         (ARM debug)
        [RecastNavigation]/qnx/Detour/x86/a                 (x86 simulator release)
        [RecastNavigation]/qnx/Detour/x86/a.g               (x86 simulator debug)
        
     libDetourCrowd: 
        [RecastNavigation]/qnx/DetourCrowd/arm/a.le.v7      (ARM release)
        [RecastNavigation]/qnx/DetourCrowd/arm/a.le.v7.g    (ARM debug)
        [RecastNavigation]/qnx/DetourCrowd/x86/a            (x86 simulator release)
        [RecastNavigation]/qnx/DetourCrowd/x86/a.g          (x86 simulator debug)

    libDetour: 
        [RecastNavigation]/qnx/Recast/arm/a.le.v7           (ARM release)
        [RecastNavigation]/qnx/Recast/arm/a.le.v7.g         (ARM debug)
        [RecastNavigation]/qnx/Recast/x86/a                 (x86 simulator release)
        [RecastNavigation]/qnx/Recast/x86/a.g               (x86 simulator debug)
        
Building from Command-line: from Momentics IDE:

    - Right click on Project Explorer->Import.
    - Select Existing Existing Project into Workspace->Next
    - Select root directory: as [RecastNavigation] 
    - Check the "Detour", "DetourCrowd" and "Recast" projects (without copying project option). Then click Finish.
    - Right click the "Detour" project then Build.
    - Right click the "DetourCrowd" project then Build.
    - Right click the "Recast" project then Build.


## Bug Reporting and Feature Requests

If you find a bug in a Sample, or have an enhancement request, simply file an [Issue](https://github.com/blackberry/RecastNavigation/issues) and send a message (via github messages) to the Committers to the project to let them know that you have filed an [Issue](https://github.com/blackberry/RecastNavigation/issues).

## Disclaimer

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

