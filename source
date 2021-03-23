#include<iostream>
#include<iomanip>
#include<string>

using namespace std;

class Time
{
private:
    int hour;
    int minute;
    int second;
public:

    //constructor with default value 0
    Time(int h = 0, int m = 0, int s = 0);

    //setter function 
    void setTime(int h, int m, int s);

    //print description of object in hh:mm:ss
    void print();

    //compare two time object
    bool equals(Time);
    int equals2(Time);

    void Display()
    {
        cout << " " << hour << ":" << minute << ":" << second << " " << endl;
    }
    int Jam3()
    {
        minute = minute + hour * 60;
        return minute;
    }
};

Time::Time(int h, int m, int s)
{
    hour = h;
    minute = m;
    second = s;
}

void Time::setTime(int h, int m, int s)
{
    hour = h;
    minute = m;
    second = s;
}

void Time::print()
{
    cout << setw(2) << setfill('0') << hour << ":"
        << setw(2) << setfill('0') << minute << ":"
        << setw(2) << setfill('0') << second << "\n";
}

int Time::equals2(Time otherTime)
{
    minute + hour * 60;
        return minute;
    
}

class Train : public Time
{
private:

    int Number;
    string Direction;
    
public:
    void setNumber(int n);
    void setDirection(string d);
    
    
    Train(int h, int m, int s, int n, string d):Time(h,m,s)
    {
        Number = n;
        Direction = d;
    }

    void Display()
    {
        
        cout << Number << " " << Direction << " " << "--->";
        Time::Display();
    }
};


void Train::setNumber(int n)
{
    Number = n;
}
void Train::setDirection(string d) 
{
    Direction = d;
};


int main()
{
    
    int mins, j, r = 0;

    

    cout << "this is our train time table today" << endl << endl;

    Train s1(2, 3, 12, 1, "sousse");
    s1.Display();
    Train s2(4, 5, 40, 2, "moscow");
    s2.Display();
    Train s3(9, 10, 33, 3, "istanbul");
    s3.Display();
    Train s4(10, 50, 11, 4, "tunis");
    s4.Display();
    Train s5(11, 12, 44, 5, "mahdia");
    s5.Display();

    cout << "Enter the time now: (h,m,s) ";
    int hr, min, sec;
    cin >> hr >> min >> sec;
    mins = hr * 60 + min;

    /*Time a1;
    a1.setTime(hr, min, sec);
    a1.Jam3();

    s1.Jam3();

    cout << s1.equals2(s2);*/

    //j = s1.Jam3() - mins;
    //cout << "number of minutes to the train number 1 is :" << j;


    int number;

    cout << "Enter the train number that you wish to know how much minutes to the departure time: ";
    cin >> number;

    if (number == 1) {
        j = s1.Jam3() - mins;
        cout << "number of minutes to the train number 1 is :" << j << " Minutes" << endl;
    }
    else if (number == 2)  {
        j = s2.Jam3() - mins;
        cout << "number of minutes to the train number 2 is :" << j << " Minutes" << endl;
    }
    else if (number == 3) {
        j = s3.Jam3() - mins;
        cout << "number of minutes to the train number 3 is :" << j << " Minutes" << endl;
    }
    else if (number == 4) {
        j = s4.Jam3() - mins;
        cout << "number of minutes to the train number 4 is :" << j << " Minutes" << endl;
    }
    else if (number == 5) {
        j = s5.Jam3() - mins;
        cout << "number of minutes to the train number 5 is :" << j << " Minutes" << endl;
    }




    //Time a1(10, 50, 59);
    //a1.print();  // 10:50:59

    //Time t2;  //object created with default value
    // // t2.print();  // 00:00:00


    //t2.setTime(10, 50, 59); //set the new time in object
    //t2.print();  // 06:39:09

    //if (t1.equals(t2))
    //    cout << "Two objects are equals\n";
    //else
    //    cout << "Two objects are not equals\n";

    return 0;
}


