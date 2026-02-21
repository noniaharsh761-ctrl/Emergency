notes and syntax of android studio 


notes of flutter
var time = final time = DateTime.now();

child: Text("current time : $time", style: TextStyle(fontSize: 25)), it will tell the date time in detail even ms 
setState(){} - it will call the build function and get the new content when it will be used , used through button 

then if we want time as in year then --> ${time.year} 
${time.weekday} - it will tell the weekend 
${time.hour}:${time.minutes}

format date :-- search intl dart flutter in google get the dependency then add it on the pub.yaml -> dev dependencies then import in the main.dart then 

${DateFormat('Hms').format(time)}  you will get the hms and all other code from the dateformat file 

date picker in flutter --> 

onPressed: () async {
                DateTime? dateoicker = await showDatePicker(
                  context: context,
                  firstDate: DateTime(2025),
                  lastDate: DateTime(2027),
                ); 


                same as showTimePicker 
                initiial time : TimeOfDay.now()
                initialEntryMode  : TimepickerEntrynmode.input ;  -- used to get the theme to select the tim elike in dialer or am pm 
                
