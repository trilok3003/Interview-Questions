1.log() :

The console.log() method is used to display message in the output web console, that is string, array or objects.

console.log('JavaScript Console');
//Output JavaScript Console
2.Error():

The error() method writes an error message to the console. The console is useful for testing purposes.

console.error('Error message');
//Error message (in danger color)

3.Warn():

The warn() method is used to display warning message to console.

console.log('Warning message');
//Warning message (in Warn type)

4.Assert():

The assert() method is used to writes an error message to the console if a assertion if false

console.assert(5+6 = 14,'Expression return wrong');
//Assertion faild :Expression return wrong 
5.Table():

The Table() method to writes a tabular data as a table.

console.table([
    {
        "id": 1,
        "first_name": "Veena",
        "last_name": "Roy",
        "class": "Class 7"
    },
    {
        "id": 2,
        "first_name": "Hari",
        "last_name": "Hara",
        "class": "Class 2"
    },
    {
        "id": 3,
        "first_name": "Pavan",
        "last_name": "Doe",
        "class": "Class 4"
    }
])
//Output


6.Count():

This Count() method Logs the number of times that this particular call to count() has been called.

for(let x =0;x<8;x++){
  console.count();
}

//Output
default: 1
default: 2
default: 3
default: 4
default: 5
default: 6
default: 7
default: 8
7.Clear():

This Clear() method Clears the console.

console.clear();
//Output Console was cleared

