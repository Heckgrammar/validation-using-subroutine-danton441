            string firstName, lastName, username, password, emailAddress;
            int age;

            // get the user inputs until all are valid.
            // The username should only be output once
            Console.Write("Enter first name: ");
            firstName = Console.ReadLine();
            ValidName(firstName);
            if (ValidName(firstName) == true)
            {


                Console.Write("Enter last name: ");
                lastName = Console.ReadLine();
                if (ValidName(lastName) == true)
                {


                    Console.Write("Enter age: ");
                    age = Convert.ToInt32(Console.ReadLine());
                    if (validAge(age) == true)
                    {
                        Console.Write("Enter Password: ");
                        password = Console.ReadLine();
                        if (ValidPassword(password) == true)
                        {

                        }
                        Console.Write("Enter email address: ");
                        emailAddress = Console.ReadLine();
                        if(validEmail(emailAddress) == true)
                        {
                            username = createUserName(firstName, lastName, age);
                            Console.WriteLine($"Username is {username}, you have successfully registered please remember your password");
                        }

                    }
                }
            }
            int asciiVal = 65 + loop(string asciiVal) > 90 || 97 + loop(asciiVal) > 122;



            username = createUserName(firstName,lastName,age);
            Console.WriteLine($"Username is {username}, you have successfully registered please remember your password");

            //  Test your program with a range of tests to show all validation works
            // Show your evidence in the Readme

        }
        static string[] loop(string[] value)
        {
            for (int i = 0; i < value; i++)
            {

            }
        }
        static bool ValidName(string name)
        {
            // name must be at least two characters and contain only letters
            int nameVal = Convert.ToInt32(name);
            if (nameVal > 65 || nameVal < 90 ||nameVal > 97 || nameVal < 122)
            {
                return true;
            }
            return false;
        }

        static bool validAge(int age)
        {
            //age must be between 11 and 18 inclusive
            if (age < 11 && 18 > age)
            {
                return true;
            }
            return false;
        }


   
        static bool ValidPassword(string password)
        {
            // Check password is at least 8 characters in length


            // Check password contains a mix of lower case, upper case and non letter characters
            // QWErty%^& = valid
            // QWERTYUi = not valid
            // ab£$%^&* = not valid
            // QWERTYu! = valid
            int asciiVal = 65 + loop(string asciiVal) > 90 || 97 + loop(asciiVal) > 122;
            if (loop(password[loop(i)]) == true)
            {
                return true;
            }
            return false;

            // Check password contains no runs of more than 2 consecutive or repeating letters or numbers
            // AAbbdd!2 = valid (only 2 consecutive letters A and B and only 2 repeating of each)
            // abC461*+ = not valid (abC are 3 consecutive letters)
            // 987poiq! = not valid (987 are consecutive)



        }
        static bool validEmail(string email)
        {
            // a valid email address
            // has at least 2 characters followed by an @ symbol
            // has at least 2 characters followed by a .
            // has at least 2 characters after the .
            // contains only one @ and any number of .
            // does not contain any other non letter or number characters
            if (email[loop(i) == loop(int asciiVal = 65 + loop(string asciiVal) > 90 || 97 + loop(asciiVal) > 122])
            {
                return true;

            }
            return false;
