
package realcase;
import java.awt.Dimension;
import java.awt.event.*;
import java.awt.*;
import javax.swing.*;
public class Customer extends JFrame implements ActionListener{
    String[] currencies={"USD","EURO","POUND","YEN","DINAR"};
    Double[] exchangeRates={55.44,61.13,69.78,0.41,181.02};


 JButton Cbutton;
JTextField field,convertedCur;
JLabel label1,label2 ;
JComboBox combo ;
    Customer(){
      convertedCur = new JTextField();
convertedCur.setPreferredSize(new Dimension(250,40));
convertedCur.setForeground(Color.green);
convertedCur.setFont(new Font("Consolas",Font.BOLD,15));
convertedCur.setBackground(Color.BLACK);
convertedCur.setEditable(false);

label2 = new JLabel("ENTER AMMOUNT:");
label2.setPreferredSize(new Dimension(250,40));
label2.setFont(new Font("Consolas",Font.BOLD,30));
label1 = new JLabel("CURRENCY:");
label1.setPreferredSize(new Dimension(200,40));
label1.setFont(new Font("Consolas",Font.BOLD,30));

combo = new JComboBox(currencies);
combo.setFont(new Font("Consolas",Font.BOLD,30));
combo.addActionListener(this);

field = new JTextField();
field.setPreferredSize(new Dimension(250, 30));
field.setForeground(Color.green);
field.setFont(new Font("Consolas",Font.BOLD,30));
field.setBackground(Color.BLACK);

Cbutton = new JButton("CONVERTED");
Cbutton.setEnabled(false);
Cbutton.addActionListener(this);

this.setLayout(new FlowLayout());
this.setTitle("CUSTOMER");
this.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
this.setSize(500,500);this.setLocationRelativeTo(null);
this.add(label2);this.add(field);

this.add(label1);
this.add(combo);



this.add(Cbutton);
this.add(convertedCur);
this.setVisible(true);

 this.pack();
  
    
    }

    @Override
    public void actionPerformed(ActionEvent e) {
         String selectedOption = (String)combo.getSelectedItem();

if(field.getText().isEmpty()){

JOptionPane.showMessageDialog(null,"ENTER AMMOUNT!!!!!" );
}
switch(selectedOption){
case "USD":
double convertedDol = Double.parseDouble(field.getText())*exchangeRates[0];
convertedCur.setText(Double.toString(convertedDol));
JOptionPane.showMessageDialog(null,"CONVERTED SUCCESSFULY!! CLAIM " + convertedDol + " PESOS");
break;
case"EURO":
double convertedEuro = Double.parseDouble(field.getText())*exchangeRates[1];
convertedCur.setText(Double.toString(convertedEuro));
JOptionPane.showMessageDialog(null,"CONVERTED SUCCESSFULY!! CLAIM " + convertedEuro + " PESOS");
break;
case"POUND":
double convertedPound = Double.parseDouble(field.getText())*exchangeRates[2];
 convertedCur.setText(Double.toString(convertedPound));
JOptionPane.showMessageDialog(null,"CONVERTED SUCCESSFULY!! CLAIM " + convertedPound + " PESOS");
 break;
case"YEN":
double convertedYen = Double.parseDouble(field.getText())*exchangeRates[3];
convertedCur.setText(Double.toString(convertedYen));
JOptionPane.showMessageDialog(null,"CONVERTED SUCCESSFULY!! CLAIM " + convertedYen + " PESOS");
break;
case "DINAR":
double convertedDinar = Double.parseDouble(field.getText())*exchangeRates[4];
convertedCur.setText(Double.toString(convertedDinar));
JOptionPane.showMessageDialog(null,"CONVERTED SUCCESSFULY!! CLAIM " + convertedDinar + " PESOS");
break;
    }
int ch= JOptionPane.showConfirmDialog(null,"DO YOU WANT TO USE AGAIN?", "TITLE", JOptionPane.YES_NO_OPTION);
 if (ch==0){
 new HomePage();
this.dispose();
}else if (ch==1)
{
 this.dispose();
 JOptionPane.showMessageDialog(null,"THANK YOU FOR USING TARLAC STATE UNIVERSITY CURRENCY CONVERTER SYSTEM");

}
    }
    
}
