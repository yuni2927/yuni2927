using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Windows.Forms;

namespace ukk2024_TEGUH
{
    public partial class Form1 : Form
    {
        decimal bil1;
        decimal bil2;
        int opr;
        Boolean opr_selesai = false;
        public Form1()
        {
            InitializeComponent();
        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void btnkoma_Click(object sender, EventArgs e)
        {
            if (textBox1.Text.Contains(',') == false)
            {
                textBox1.Text = textBox1.Text + ",";
            }
        }

        private void btn0_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text = "0";
            }
            else
            {
                textBox1.Text += "0";
            }

        }


        private void btn1_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text += "1";
            }
            else
            {
                textBox1.Text = "1";
            }

        }

        private void btn2_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text += "2";
            }
            else
            {
                textBox1.Text = "2";
            }

        }

        private void btn3_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text += "3";
            }
            else
            {
                textBox1.Text = "3";
            }

        }

        private void btn4_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text = "4";
            }
            else
            {
                textBox1.Text += "4";
            }

        }

        private void btn5_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text = "5";
            }
            else
            {
                textBox1.Text += "5";
            }

        }

        private void btn6_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text = "6";
            }
            else
            {
                textBox1.Text += "6";
            }

        }

        private void btn7_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text = "7";
            }
            else
            {
                textBox1.Text += "7";
            }

        }

        private void btn8_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text += "8";
            }
            else
            {
                textBox1.Text += "8";
            }

        }

        private void btn9_Click(object sender, EventArgs e)
        {
            if (textBox1.Text == "0")
            {
                textBox1.Text = "9";
            }
            else
            {
                textBox1.Text += "9";
            }

        }

        private void btnkali_Click(object sender, EventArgs e)
        {
            bil1 = Convert.ToDecimal(textBox1.Text);

            textBox1.Text = "*";
            textBox2.Text = "";
            opr = 1;
            opr_selesai = true;



        }

        private void btntambah_Click(object sender, EventArgs e)
        {
            bil1 = Convert.ToDecimal(textBox1.Text);

            textBox1.Text = "+";
            textBox2.Text = "";
            opr = 2;
            opr_selesai = true;

        }

        private void btnbagi_Click(object sender, EventArgs e)
        {
            bil1 = Convert.ToDecimal(textBox1.Text);

            textBox1.Text = "/";
            textBox2.Text = "";
            opr = 3;
            opr_selesai = true;

        }

        private void btnkurang_Click(object sender, EventArgs e)
        {
            bil1 = Convert.ToDecimal(textBox1.Text);

            textBox1.Text = "-";
            textBox2.Text = "";
            opr = 4;
            opr_selesai = true;

        }

        private void btnsd_Click(object sender, EventArgs e)
        {
            if (opr_selesai == true)
                bil2 = Convert.ToDecimal(textBox1.Text);
            {
                switch (opr)
                {
                    case 1:
                        textBox1.Text = Convert.ToString(bil1 * bil2);
                        break;
                    case 2:
                        textBox1.Text = Convert.ToString(bil1 + bil2);
                        break;
                    case 3:
                        textBox1.Text = Convert.ToString(bil1 / bil2);
                        break;
                    case 4:
                        textBox1.Text = Convert.ToString(bil1 - bil2);
                        break;

                }
            }
        }

        private void btnhapus_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text.Remove(textBox1.Text.Length - 1);
            if ((textBox1.Text == "") || (textBox1.Text == "-"))
            {
                textBox1.Text = "0";
            }
        }

        private void btnc_Click(object sender, EventArgs e)
        {
            textBox1.Text = "0";
            bil1 = 0;
            bil2 = 0;
            textBox2.Text = "";
        }
    }

}

      

      
        
        

        


         

        
- 👋 Hi, I’m @yuni2927
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
yuni2927/yuni2927 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
