namespace calculator
{
    public partial class Form1 : Form
    {
        string opr;
        Double oparand1, oparand2;
        bool clearDisplay = false;
        public Form1()
        {
           
            InitializeComponent();
        }

        private void buttongr_Click(object sender, EventArgs e)
        {

        }

        private void button0_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + "0";

            }
            else
            {
                this.textBox2.Text = "0";
            }
            clearDisplay = false;
        }

        private void button1_Click(object sender, EventArgs e)
        {
            if(clearDisplay== false)
            {
                this.textBox2.Text = this.textBox2.Text + "1";

            }
           
            clearDisplay = false;
        }

        private void button3_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + "3";

            }
            else
            {
                this.textBox2.Text = "3";
            }
            clearDisplay = false;
        }

        private void button4_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + "4";

            }
            else
            {
                this.textBox2.Text = "4";
            }
            clearDisplay = false;
        }

        private void button5_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + "5";

            }
            else
            {
                this.textBox2.Text = "5";
            }
            clearDisplay = false;
        }

        private void button6_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + "6";

            }
            else
            {
                this.textBox2.Text = "6";
            }
            clearDisplay = false;
        }

        private void button7_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + "7";

            }
            else
            {
                this.textBox2.Text = "7";
            }
            clearDisplay = false;
        }

        private void button8_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + "8";

            }
            else
            {
                this.textBox2.Text = "8";
            }
            clearDisplay = false;
        }

        private void button9_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + "9";

            }
            else
            {
                this.textBox2.Text = "9";
            }
            clearDisplay = false;
        }

        private void buttonmult_Click(object sender, EventArgs e)
        {

            oparand1 = Convert.ToDouble(this.textBox2.Text);
            opr = "*";
            clearDisplay = true;
        }

        private void buttonc_Click(object sender, EventArgs e)
        {
            this.textBox2.Clear();
            this.textBox2.Text = "0";
        }

        private void buttonmies_Click(object sender, EventArgs e)
        {
            oparand1 = Convert.ToDouble(this.textBox2.Text);
            opr = "-";
            clearDisplay = true;
        }

        private void buttondivied_Click(object sender, EventArgs e)
        {
            oparand1 = Convert.ToDouble(this.textBox2.Text);
            opr = "/";
            clearDisplay = true;
        }

        private void buttonequel_Click(object sender, EventArgs e)
        {
            double result;
            oparand2 = Convert.ToDouble(this.textBox2.Text);
            switch (opr)
            {
                case "+":
                    result = oparand1 + oparand2;
                    textBox2.Text = Convert.ToString(result);
                    break;
                case "-":
                    result = oparand1 - oparand2;
                    textBox2.Text = Convert.ToString(result);
                    break;
                case "*":
                    result = oparand1 * oparand2;
                    textBox2.Text = Convert.ToString(result);
                    break;
                case "/":
                    if (oparand2 == 0)
                    {
                        textBox2.Text = "0.0";
                        break;
                    }
                    else
                    {
                        result = oparand1 / oparand2;
                        textBox2.Text = Convert.ToString(result);
                        break;
                    }
                case "%":
                    result = oparand1 % oparand2;
                    textBox2.Text = Convert.ToString(result);
                    break;
            }
        }

        private void buttonpoint_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + ".";

            }
            else
            {
                this.textBox2.Text = ".";
            }
            clearDisplay = false;
        }

        private void button2_Click(object sender, EventArgs e)
        {
            if (clearDisplay == false)
            {
                this.textBox2.Text = this.textBox2.Text + "2";

            }
            
            clearDisplay = false;
        }

        private void textBox2_TextChanged(object sender, EventArgs e)
        {

        }

        private void buttonadd_Click(object sender, EventArgs e)
        {
            oparand1= Convert.ToDouble(this.textBox2.Text);
            opr = "+";
            clearDisplay = true;
            
        }
        
    }
}
