# helloWorld
My first.

This is my first commit and I hope it will be helpfull to someone else and also remind me of when it all started! 

So this is my solution for a common problem that is solved by students when learning to code - Leap Year identifier.


It is written in X-code 12.0.1 and using SWIFT 5.3.
Of course it is simple but it's tricky and I havent found a decent answer to this question, so as a result - here we go:
Put it into playgrounds, call the checkLeapYear function passing a year into it and play around.

func checkLeapYear(year: Int) {
    if year % 4 == 0{
        if year % 100 == 0 {
            if year % 400 == 0{
                print("\(year) is a Leap Year!")
            } else {
                print("\(year) is NOT a Leap Year!")
            }
        } else {
            print("\(year) is a Leap Year!")
        }
    } else {
        print("\(year) is NOT a Leap Year!")
    }
}

The algorithm is quite tricky so I suggest you use the following logic when performing it on your own:
1. If the year is evenly divisible by 4, go to step 2.   Otherwise, go to step 5.
2. If the year is evenly divisible by 100, go to step 3.   Otherwise, go to step 4.
3. If the year is evenly divisible by 400, go to step 4.   Otherwise, go to step 5.
4. The year is a leap year.
5. The year is not a leap year.
