# Local Storage and How To Use It On Websites

**Why would a developer use local storage for a web application?**
Local storage allows a devloper to store small pieces of user information by storing it locally (on their machine). This way, when the user returns, they won;'t have to go through all of the steps they already went through, and can more quickly access other elements of the application.

**What information should not be stored in local storage?**
Sensitive information, such as username and passord, should not be stored locally. Instead, it should be stored on the back-end.

**Local storage can store what type of data? How would you convert it to that type before storing?**
Loacl storage can only store stings. To get around this, one can use the native JSON.stringify() and JSON.parse() methods.
