#DATE_TIME

var value = new Date ("December, 30,2000 20:00:00");
var donustur = String(value);
var parcala = donustur.split(" ");
var birinciDeger = parcala[0];

getFullYear()    getUTCFullYear()         : 1000 - 9999          setFullYear()       setUTCFullYear()       : 1000 - 9999   Çoklu ayarlama işlemi yapılabilir (2053 , 12 , 31)
getMonth()       getUTCMonth()            : 0 - 11               setMonth()          setUTCMonth()          : 0 - 11        Çoklu ayarlama işlemi yapılabilir (11 , 31)
getDate()        getUTCDate()             : 1 - 31               setDate()           setUTCDateİ()          : 1 - 31
getDay()         getUTCDay()              : 0 - 6 (Sunday)
getHours()       getUTCHours()            : 0 - 23               setHours()          setUTCHours()          : 0 - 23        Çoklu ayarlama işlemi yapılabilir (23 , 59, 59, 999)
getMinutes()     getUTCMinutes()          : 0 - 59               setMinutes()        setUTCMinutes()        : 0 - 59        Çoklu ayarlama işlemi yapılabilir (59, 59, 999)
getSeconds()     getUTCSeconds()          : 0 - 59               setSeconds()        setUTCSeconds()        : 0 - 59        Çoklu ayarlama işlemi yapılabilir (59, 999)
getMilliseconds  getUTCMilliseconds()     : 0 - 999              setMilliseconds()   setUTCMilliseconds()   : 0 - 999

getTime()        getUTCTime()                                    setTime()           setUTCTime()           : Zaman Damgası (Time Stamp, GMT 'dir.) // 01.01.1970 GMT +02:00
now()                                                            UTC(2053, 12, 31,  23, 59, 59, 999)        : Date.now()  (Time Stamp, UTC 'dir.) // 01.01.1970 GMT +02:00

parse()                     : (SetDate - TimeStamp)              let fark = Date.parse("July 5, 1975");     // Parametre Sıralaması (Ay(İnglizce), Gün, Yıl, Saat:Dakika:Saniye:MiliSaniye)
getTimeZoneOffset()         : (GMT (LocalTime) - GMT (0) ) = value type minute 
toString()                  : Converting typeof String
toLocaleString()            : Converting Locale typeof String
toUTCString()               : Converting UTC typeof String
toISOString()               : Converting ISO typeof String
toJSON()                    : Converting time and date object to change JSon typeof String
toDateString()              : Select Date (Tarih) and convert to toString
toLocaleDateString()        : toDateString + toLocaleString
toTimeString()              : Select Time (Saat) and convert to toString
toLocaleTimeString()        : toTimeString + toLocaleString
valueOf()                   : convert to TimeStamp and typeof Number
