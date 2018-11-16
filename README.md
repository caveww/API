>        [DllImport(V, CharSet = CharSet.Unicode)]
>        public static extern string MSGBoxC(string TITLE, string MESSAGE);

>        MSGBoxC("hello", "test");
***
>         [DllImport("EZAPI-V1.dll", CharSet = CharSet.Unicode)]
>         public static extern void SleepC(int TIME);

>         SleepC(5000); //5000 = 5 sec
***
>         [DllImport("EZAPI-V1.dll", CharSet = CharSet.Unicode)]
>         public static extern void ExitC(int CODE);

>         ExitC(10); //exit the program and return a value of 10
***
>         [DllImport("EZAPI-V1.dll", CharSet = CharSet.Unicode)]
>         public static extern void MessageC(string MESSAGE);

>         MessageC("hello");
***
>         [DllImport("EZAPI-V1.dll", CharSet = CharSet.Unicode)]
>         public static extern string GetHwid();

>         GetHwid(); //return to a value
***
>         [DllImport("EZAPI-V1.dll", CharSet = CharSet.Unicode)]
>         public static extern string MakeFileC(string FILENAME, string WRITE);

>         MakeFileC("test.txt", "Hello Every one");
***
>         [DllImport("EZAPI-V1.dll", CharSet = CharSet.Unicode)]
>         public static extern string FTP(string HOST, string USER, string PASSWORD, int PORT, string FILE, string FILEDESTINATION);

>         FTP("Google.com", "user12340", "password12340", 21, "test.txt", "LOGS/test.txt"); // default Port is 21
***
>`MSGBoxC` - `        public static extern string MSGBoxC(string TITLE, string MESSAGE);` - `TITLE` is the textbox title - `MESSAGE` is the textbox message - ex; `MSGBoxC("hello", "test");`
***
>`SleepC` - `public static extern void SleepC(int TIME);` - `TIME` amount of time  - ex; `SleepC(5000);`

***

>`ExitC` - `public static extern void ExitC(int CODE);` - `CODE` exit the program and return a value of 10 - ex; `ExitC(10);`

***

>`MessageC` - `public static extern void MessageC(string MESSAGE);` - `MESSAGE` string message - ex; `MessageC("hello");`

***

>`GetHwid` - `public static extern string GetHwid();` - `GetHwid();` return to a value

***

>`MakeFileC` - `public static extern string MakeFileC(string Filename, string WRITE);` - `FILENAME` the name of the file to make - `WRITE` stuff that you want to write in the file - ex; `MakeFileC("test.txt", "Hello Every one");`

***

>`FTP` - `public static extern string FTP(string HOST, string USER, string PASSWORD, int PORT, string FILE, string FILEDESTINATION);` - `HOST` host name like google.com but put your own - `USER` the ftp username - `PASSWORD` the password of the ftp server (client) - `PORT` the port of the server the default Port is 21 - `FILE` the file to upload - `FILEDESTINATION` the destination file in the ftp server (client) - ex; `FTP("Google.com", "user12340", "password12340", 21, "test.txt", "LOGS/test.txt"); // default Port is 21`
