# Anastasiia Zubareva
"resource": [
  {
    "files" : [
      "**/*.png",
      "**/*.jpg,
      "**/*.gif"
    ],
![me](C:\Users\79134\Downloads\Telegram Desktop\me.jpg)
## Contact
* +79134530408
* foolmaak@gmail.com
* telegram: u23571113u
## About me
I studing C++/C# programming and I want to progress as a frontend developer. My goal is to learn new.
## Skills
* C++/C# (Basic)
* JavaScript (Basic)
* VS Code
* Git
## Code Example
namespace ClassLibraryModel
{
    public class Calculation
    {
        public string FirstOperand { get; set; } = "";
        public string SecondOperand { get; set; } = "";
        public string Operation { get; set; } = "";
        public string Result { get; private set; } = "";

        public Calculation() { }

        public Calculation(string firstOperand, string secondOperand, string operation) {
            CheckOperand(firstOperand);
            CheckOperand(secondOperand);
            CheckOperator(operation);
            FirstOperand = firstOperand;
            SecondOperand = secondOperand;
            Operation = operation;
        }

        public void Calculate() {
            CheckOperand(FirstOperand);
            CheckOperand(SecondOperand);
            CheckOperator(Operation);
            try
            {
                switch (Operation)
                {
                    case "+":
                        Result = (Convert.ToDouble(FirstOperand) + Convert.ToDouble(SecondOperand)).ToString();
                        break;
                    case "-":
                        Result = (Convert.ToDouble(FirstOperand) - Convert.ToDouble(SecondOperand)).ToString();
                        break;
                    case "*":
                        Result = (Convert.ToDouble(FirstOperand) * Convert.ToDouble(SecondOperand)).ToString();
                        break;
                    case "/":
                        if (SecondOperand == "0")
                        {
                            Result = "Zero devision error";
                            throw new ArgumentException("Zero devision error");
                        }
                        Result = (Convert.ToDouble(FirstOperand) / Convert.ToDouble(SecondOperand)).ToString();
                        break;
                }
            }
            catch
            {
                Result = "Unknow error";
                throw;
            }

        }

        protected virtual void CheckOperator(string operation)
        {
            switch(operation){
                case "+":
                case "-":
                case "*":
                case "/":
                    break;
                default:
                    Result = "Operation Error";
                    throw new ArgumentException("Operation Error");
            }
        } 

        private void CheckOperand(string operand)
        {
            try
            {
                Convert.ToDouble(operand);
            }
            catch
            {
                Result = "Operation Error";
                throw;
            }
        }
    }
}
## Education
* CI.NSU
+ incomplete secondary special
* RS School
+ JS/Frontend. Stage 0
## English
* B1