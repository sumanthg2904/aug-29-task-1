# aug-29-task-1
This Repo Contains tasks files and folders
1. Created the new repo in the git hub 
   name : aug-29-task-1

2. Add the java program 
   I created the factorial program 
      - class factorial{  
              static int factorial(int n){    
                        if (n == 0)    
                           return 1;    
                        else    
                           return(n * factorial(n-1));    
                      }    
        public static void main(String args[]){  
        int i,fact=1;  
        int number=4;//It is the number to calculate factorial    
        fact = factorial(number);   
        System.out.println("Factorial of "+number+" is: "+fact);    
        }  
     }  

   * to compile the program i use the command as 
     javac factorial.java
   * to run the program
     java factorial
3. Create a new jenkins freestyle project
   -- i created the new job in jenkins named as
      name : factorial project
   -- check out the git repo.
      i check the repo by cloning the repo by using 
      Source Code Management
      i selected the git and i configured it.
   -- compile and run the java program.
      by selecting the -> Build Steps
                          Execute shell
                             ->  to compile 
                                 javac factorial.java
                             ->  to run the program
                                 java factorial

    1. Task 2
    2. Add the java program 
   
        class calculator {
    public static void main(String[] args) {
        if (args.length < 3) {
            System.out.println("Usage: java SimpleCalculator <operation> <num1> <num2>");
            return;
        }

        int choice = Integer.parseInt(args[0]);
        double num1 = Double.parseDouble(args[1]);
        double num2 = Double.parseDouble(args[2]);

        double result = 0;
        
        switch (choice) {
            case 1:
                result = num1 + num2;
                break;
            case 2:
                result = num1 - num2;
                break;
            case 3:
                result = num1 * num2;
                break;
            case 4:
                if (num2 != 0) {
                    result = num1 / num2;
                } else {
                    System.out.println("Error: Division by zero is not allowed.");
                    return;
                }
                break;
            default:
                System.out.println("Invalid choice.");
                return;
        }

        System.out.println("Result: " + result);
    }
}

   * to compile the program i use the command as 
     javac calculator.java   * to run the program
     java calculator (opt: 1) (num1: 20) + (num2: 30)


3. Create a new jenkins freestyle project
   -- i created the new job in jenkins named as
      name : calculator project
   -- check out the git repo.
      i check the repo by cloning the repo by using 
      Source Code Management
      i selected the git and i configured it.
   -- compile and run the java program.
      by selecting the -> Build Steps
                          Execute shell
                             ->  to compile 
                                 javac calculator.java
                             ->  to run the program
                                 java calculator (opt: 1) (num1: 20) + (num2: 30)
   4. merging the calci branch and master branch.
      git branch calci
      git checkout calci
      git merge master

 		 

