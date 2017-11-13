using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows;
using System.Windows.Controls;
using System.Windows.Data;
using System.Windows.Documents;
using System.Windows.Input;
using System.Windows.Media;
using System.Windows.Media.Imaging;
using System.Windows.Navigation;
using System.Windows.Shapes;

namespace Bucky
{
    /// <summary>
    /// Interaction logic for MainWindow.xaml
    /// </summary>
    public partial class MainWindow : Window
    {
        public MainWindow()
        {
            InitializeComponent();
        }

        private void button_Click(object sender, RoutedEventArgs e)
        {
            int b;
            int[] array = new int[28];
            array[0] = 0;
            array[1] = 1;
            for (int i =0; i<=28; i++)
            {
                array[i+2] = array[i] + array[i + 1];
                b = array[i + 2];
                MessageBox.Show(b.ToString());
            }
        }
    }
}
