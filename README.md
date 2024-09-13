//main
GetEnjoymentLevel();
string stadiumRec = GetStadiumRecommendation();
while (stadiumRec != "5"){
    RouteEm(stadiumRec);
    GetEnjoymentLevel();
    stadiumRec = GetStadiumRecommendation();
}
//end main


static void GetEnjoymentLevel(){
    Console.Clear();
    System.Console.WriteLine ("What enjoyment level would you like? \n1. Boring\n2. Average\n3. Fun\n4. Epic \n5. Exit");
}


static string GetStadiumRecommendation(){
    System.Console.WriteLine("Enter your choice");
    return Console.ReadLine();
}


static void RouteEm(string stadiumRec){
    switch (stadiumRec)
    {
    case "1":
        GoToNeyLand();
        break;
    case "2":
        GoToJordanHare();
        break;
    case "3":
        GoToTigerStadium();
        break;
    case "4":
        GoToBryantDenny();
        break;
    case "5":
        SayGoodBye();
        break;
    default:
        System.Console.WriteLine("Invalid choice");
        Pause();
        break;
    }
}


static void GoToNeyLand(){
    System.Console.WriteLine("You should go to Neyland stadium");
    System.Console.WriteLine("Would you like a game reccomendation?");
    string neyland = Console.ReadLine().ToLower();
        if(neyland == "yes"){
            System.Console.WriteLine("Go to the kent state game");
            }
        if(neyland == "no"){
            Pause();
        }
            Pause();


    }


static void GoToJordanHare(){
    System.Console.WriteLine("You should go to Jordan hare");
    System.Console.WriteLine("Would you like a game reccomendation?");
    string hare = Console.ReadLine().ToLower();
        if(hare == "yes"){
            System.Console.WriteLine("Go to the kentucky game");
            }
        if(hare == "no"){
            Pause();
        }
            Pause();
}




static void GoToTigerStadium(){
    System.Console.WriteLine("you should go to tiger stadium");
    System.Console.WriteLine("Would you like a game reccomendation?");
        string stadium = Console.ReadLine().ToLower();
        if(stadium == "yes"){
            System.Console.WriteLine("Go to the alabama game");
            }
        if(stadium == "no"){
            Pause();
        }
            Pause();
}




static void GoToBryantDenny(){
    System.Console.WriteLine("You should go to bryant denny");
    System.Console.WriteLine("Would you like a game reccomendation?");
    string denny = Console.ReadLine().ToLower();
        if(denny == "yes"){
            System.Console.WriteLine("Go to the auburn game");
            }
        if(denny == "no"){
            Pause();
        }
            Pause();
}


static void SayGoodBye(){
    System.Console.WriteLine("Goodbye!");
}


static void Pause(){
    System.Console.WriteLine("Press any key to continue..");
    Console.ReadKey();
}


