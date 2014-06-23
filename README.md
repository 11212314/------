1 Файл Main.java
package viktorina;
import java.sql.Driver;
import java.sql.DriverManager;
import java.sql.ResultSet;
import java.sql.ResultSetMetaData;
import java.util.Properties;
import javax.swing.JProgressBar;
public class Main {
 static public Object [][] data;
 static public Object [][] data2;
 static public Object [][] data3;
 static public Object [][] data4;
 static public Object [][] data5;
 static public Object [][] data6;
 static public Object [][] data7;
 static public Object [][] data8;
 static public Object [][] data9;
   static public int nomVekt;
static Properties connInfo = new Properties();
static   NewJFrame n=new NewJFrame();
static   NewJFrame1 qwe=new NewJFrame1();
       public static void WV()
    {
           int col;
           int row;
        try
        {
            Class.forName("sun.jdbc.odbc.JdbcOdbcDriver");
            java.sql.Connection con=DriverManager.getConnection("jdbc:odbc:WV",connInfo);
            java.sql.Statement stmt=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
            ResultSet rs=stmt.executeQuery("select * from psevdo");
            ResultSetMetaData rsmd=rs.getMetaData();
            col=rsmd.getColumnCount();
            rs.last();
            row=rs.getRow();
            rs.beforeFirst();
            data=new Object[row][col];
            for(int i=0;i<row;i++)
            {
                rs.next();
                for (int j=0;j<col;j++)
                {
                    data[i][j]=rs.getString(j+1);
                }
            }
            rs.beforeFirst();
            rs.close(); 
            stmt.close();
            con.close();
        }
        catch (Exception e)
        {
            System.out.println("Ошибка при инициализации базы"+e);
        }
    }
 public static void WV2()
    {
           int col;
           int row;
        try
        {
            Class.forName("sun.jdbc.odbc.JdbcOdbcDriver");
            java.sql.Connection con=DriverManager.getConnection("jdbc:odbc:WV",connInfo);
            java.sql.Statement stmt=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
            ResultSet rs=stmt.executeQuery("select * from 7");
            ResultSetMetaData rsmd=rs.getMetaData();
            col=rsmd.getColumnCount();
            rs.last();
            row=rs.getRow();
            rs.beforeFirst();
            data2=new Object[row][col];
            for(int i=0;i<row;i++)
            {
                rs.next();
                for (int j=0;j<col;j++)
                {
                    data2[i][j]=rs.getString(j+1);
                }
            }
            rs.beforeFirst();
            rs.close();
            stmt.close();
            con.close();
        }
        catch (Exception e)
        {
            System.out.println("Ошибка при инициализации базы"+e);
        }
    }
  public static void WV3()
    {
           int col;
           int row;
        try
        {
            Class.forName("sun.jdbc.odbc.JdbcOdbcDriver");
            java.sql.Connection con=DriverManager.getConnection("jdbc:odbc:WV",connInfo);
            java.sql.Statement stmt=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
            ResultSet rs=stmt.executeQuery("select * from pc");
            ResultSetMetaData rsmd=rs.getMetaData();
            col=rsmd.getColumnCount();
            rs.last();
            row=rs.getRow();
            rs.beforeFirst();
            data3=new Object[row][col];
            for(int i=0;i<row;i++)
            {
                rs.next();
                for (int j=0;j<col;j++)
                {
                    data3[i][j]=rs.getString(j+1);
                }
            }
            rs.beforeFirst();
            rs.close();
            stmt.close();
            con.close();
        }
        catch (Exception e)
        {
            System.out.println("Ошибка при инициализации базы"+e);
        }
    }
   public static void WV4()
    {
           int col;
           int row;
        try
        {
            Class.forName("sun.jdbc.odbc.JdbcOdbcDriver");
            java.sql.Connection con=DriverManager.getConnection("jdbc:odbc:WV",connInfo);
            java.sql.Statement stmt=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
            ResultSet rs=stmt.executeQuery("select * from vino");
            ResultSetMetaData rsmd=rs.getMetaData();
            col=rsmd.getColumnCount();
            rs.last();
            row=rs.getRow();
            rs.beforeFirst();
            data4=new Object[row][col];
            for(int i=0;i<row;i++)
            {
                rs.next();
                for (int j=0;j<col;j++)
                {
                    data4[i][j]=rs.getString(j+1);
                }
            }
            rs.beforeFirst();
            rs.close();
            stmt.close();
            con.close();
        }
        catch (Exception e)
        {
            System.out.println("Ошибка при инициализации базы"+e);
        }
    }
    public static void WV5()
    {
           int col;
           int row;
        try
        {
            Class.forName("sun.jdbc.odbc.JdbcOdbcDriver");
            java.sql.Connection con=DriverManager.getConnection("jdbc:odbc:WV",connInfo);
            java.sql.Statement stmt=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
            ResultSet rs=stmt.executeQuery("select * from simvol");
            ResultSetMetaData rsmd=rs.getMetaData();
            col=rsmd.getColumnCount();
            rs.last();
            row=rs.getRow();
            rs.beforeFirst();
            data5=new Object[row][col];
            for(int i=0;i<row;i++)
            {
                rs.next();
                for (int j=0;j<col;j++)
                {
                    data5[i][j]=rs.getString(j+1);
                }
            }
            rs.beforeFirst();
            rs.close();
            stmt.close();
            con.close();
        }
        catch (Exception e)
        {
            System.out.println("Ошибка при инициализации базы"+e);
        }
    }
     public static void WV6()
    {
           int col;
           int row;
        try
        {
            Class.forName("sun.jdbc.odbc.JdbcOdbcDriver");
            java.sql.Connection con=DriverManager.getConnection("jdbc:odbc:WV",connInfo);
            java.sql.Statement stmt=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
            ResultSet rs=stmt.executeQuery("select * from cities");
            ResultSetMetaData rsmd=rs.getMetaData();
            col=rsmd.getColumnCount();
            rs.last();
            row=rs.getRow();
            rs.beforeFirst();
            data6=new Object[row][col];
            for(int i=0;i<row;i++)
            {
                rs.next();
                for (int j=0;j<col;j++)
                {
                    data6[i][j]=rs.getString(j+1);
                }
            }
            rs.beforeFirst();
            rs.close();
            stmt.close();
            con.close();
        }
        catch (Exception e)
        {
            System.out.println("Ошибка при инициализации базы"+e);
        }
    }
      public static void WV7()
    {
           int col;
           int row;
        try
        {
            Class.forName("sun.jdbc.odbc.JdbcOdbcDriver");
            java.sql.Connection con=DriverManager.getConnection("jdbc:odbc:WV",connInfo);
            java.sql.Statement stmt=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
            ResultSet rs=stmt.executeQuery("select * from igra");
            ResultSetMetaData rsmd=rs.getMetaData();
            col=rsmd.getColumnCount();
            rs.last();
            row=rs.getRow();
            rs.beforeFirst();
            data7=new Object[row][col];
            for(int i=0;i<row;i++)
            {
                rs.next();
                for (int j=0;j<col;j++)
                {
                    data7[i][j]=rs.getString(j+1);
                }
            }
            rs.beforeFirst();
            rs.close();
            stmt.close();
            con.close();
        }
        catch (Exception e)
        {
            System.out.println("Ошибка при инициализации базы"+e);
        }
    }
 public static void WV8()
    {
           int col;
           int row;
        try
        {
            Class.forName("sun.jdbc.odbc.JdbcOdbcDriver");
            java.sql.Connection con=DriverManager.getConnection("jdbc:odbc:WV",connInfo);
            java.sql.Statement stmt=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
            ResultSet rs=stmt.executeQuery("select * from mechi");
            ResultSetMetaData rsmd=rs.getMetaData();
            col=rsmd.getColumnCount();
            rs.last();
            row=rs.getRow();
            rs.beforeFirst();
            data8=new Object[row][col];
            for(int i=0;i<row;i++)
            {
                rs.next();
                for (int j=0;j<col;j++)
                {
                    data8[i][j]=rs.getString(j+1);
                }
            }
            rs.beforeFirst();
            rs.close();
            stmt.close();
            con.close();
        }
        catch (Exception e)
        {
            System.out.println("Ошибка при инициализации базы"+e);
        }
    }
  public static void WV9()
    {
           int col;
           int row;
        try
        {
            Class.forName("sun.jdbc.odbc.JdbcOdbcDriver");
            java.sql.Connection con=DriverManager.getConnection("jdbc:odbc:WV",connInfo);
            java.sql.Statement stmt=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
            ResultSet rs=stmt.executeQuery("select * from bogi");
            ResultSetMetaData rsmd=rs.getMetaData();
            col=rsmd.getColumnCount();
            rs.last();
            row=rs.getRow();
            rs.beforeFirst();
            data9=new Object[row][col];
            for(int i=0;i<row;i++)
            {
                rs.next();
                for (int j=0;j<col;j++)
                {
                    data9[i][j]=rs.getString(j+1);
                }
            }
            rs.beforeFirst();
            rs.close();
            stmt.close();
            con.close();
        }
        catch (Exception e)
        {
            System.out.println("Ошибка при инициализации базы"+e);
        }
    }
    public static void main(String[] args) {

connInfo.put("user", "");
connInfo.put("password", "");
connInfo.put("charSet", "Cp1251");
  n.setVisible(true);
      WV();
      WV2();
      WV3();
      WV4();
      WV5();
      WV6();
      WV7();
      WV8();
      WV9();
    }
}

   1 Файл NewJFrame.java
package viktorina;
import java.awt.Label;
import java.util.Properties;
import viktorina.NewJFrame1;
public class NewJFrame extends javax.swing.JFrame {
    static public int clos;
    public NewJFrame() {
        initComponents();
        jLabel1.setText("Ваш прогресс: "+ jProgressBar1.getValue());
         if (NewJFrame.clos>1){
Main.qwe.setVisible(false);
        }
    }
    @SuppressWarnings("unchecked")
    private void jButton4ActionPerformed(java.awt.event.ActionEvent evt) {      
    }                                        
    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
      NewJFrame1 n=new NewJFrame1();
      n.setVisible(true);
      Main.nomVekt=1;
    }                                        
    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        NewJFrame1 n=new NewJFrame1();
      n.setVisible(true);
      Main.nomVekt=2;
    }                                        
    private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {                                         
       NewJFrame1 n=new NewJFrame1();
      n.setVisible(true);
      Main.nomVekt=3;
    }                                        
    private void jButton5ActionPerformed(java.awt.event.ActionEvent evt) {                                         
       NewJFrame1 n=new NewJFrame1();
      n.setVisible(true);
      Main.nomVekt=4;
    }                                        
    private void jButton6ActionPerformed(java.awt.event.ActionEvent evt) {                                         
       NewJFrame1 n=new NewJFrame1();
      n.setVisible(true);
      Main.nomVekt=5;
    }                                        
    private void jButton7ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        NewJFrame1 n=new NewJFrame1();
      n.setVisible(true);
      Main.nomVekt=6;
    }                                        
    private void jButton8ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        NewJFrame1 n=new NewJFrame1();
      n.setVisible(true);
      Main.nomVekt=7;
    }                                        
    private void jButton9ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        NewJFrame1 n=new NewJFrame1();
      n.setVisible(true);
      Main.nomVekt=8; }
    private void jButton10ActionPerformed(java.awt.event.ActionEvent evt) {                                          
       NewJFrame1 n=new NewJFrame1();
      n.setVisible(true);
      Main.nomVekt=9; }       
    public static void main(String args[]) {
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new NewJFrame().setVisible(true);
            }
        }); } 
    private javax.swing.JButton jButton1;
    private javax.swing.JButton jButton10;
    private javax.swing.JButton jButton2;
    private javax.swing.JButton jButton3;
    private javax.swing.JButton jButton4;
    private javax.swing.JButton jButton5;
    private javax.swing.JButton jButton6;
    private javax.swing.JButton jButton7;
    private javax.swing.JButton jButton8;
    private javax.swing.JButton jButton9;
    public static javax.swing.JLabel jLabel1;
    public static javax.swing.JProgressBar jProgressBar1;             
}

3  Файл NewJFrame1.java
package viktorina;
import java.util.Locale;
import java.util.Random;
import javax.swing.JProgressBar;
public class NewJFrame1 extends javax.swing.JFrame {
public int [] massotv=new int[4];
int Rand;
public static int nomVopr;
public int schet;
Object [][] ViktorData; 
    public NewJFrame1() {
        initComponents();
    } 
    private void formWindowOpened(java.awt.event.WindowEvent evt) {                                  
nomVopr=1;
        if (Main.nomVekt==1)
{
 ViktorData=Main.data;
}
if (Main.nomVekt==2)
{
 ViktorData=Main.data2;
}
if (Main.nomVekt==3)
{
 ViktorData=Main.data3;
}
if (Main.nomVekt==4)
{
 ViktorData=Main.data4;
}
if (Main.nomVekt==5)
{
 ViktorData=Main.data5;
}
if (Main.nomVekt==6)
{
 ViktorData=Main.data6;
}
if (Main.nomVekt==7)
{
 ViktorData=Main.data7;
}
if (Main.nomVekt==8)
{
 ViktorData=Main.data8;
}
if (Main.nomVekt==9)
{
 ViktorData=Main.data9;
}
 show_vopr(nomVopr);
    }                     
public void show_vopr(int nom)
    {
jButton5.setVisible(false);
jTextArea1.setText(ViktorData[nom-1][1]+"");
            for (int j=0;j<4;j++)
            {
             massotv[j]=0;
            }
Random r=new Random();
for(int i=0;i<4;i++)
        {
            Rand=r.nextInt(4)+1;
            for (int j=0;j<=i;j++)
            {
            if (massotv[j]==Rand)
                {
                Rand= r.nextInt(4)+1;
                j=-1;
                }
            }
            massotv[i]=Rand;
            System.out.println(massotv[i]);
         }
jButton1.setText(ViktorData[nom-1][massotv[0]+1]+"");
jButton2.setText(ViktorData[nom-1][massotv[1]+1]+"");
jButton3.setText(ViktorData[nom-1][massotv[2]+1]+"");
jButton4.setText(ViktorData[nom-1][massotv[3]+1]+"");
jTextArea2.setVisible(false);
jScrollPane2.setVisible(false);
jTextArea2.setText(ViktorData[nom-1][6]+"");
}
    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
jButton5.setVisible(true);
jTextArea2.setVisible(true);
jScrollPane2.setVisible(true);
jButton1.setVisible(false);
jButton2.setVisible(false);
jButton3.setVisible(false);
jButton4.setVisible(false);
        if (jButton1.getText().equals(ViktorData [nomVopr-1][2]))
 {
   jTextArea1.setText("Ответ верный!!!");
  NewJFrame.jProgressBar1.setValue(NewJFrame.jProgressBar1.getValue()+1);
    NewJFrame.jLabel1.setText("Ваш прогресс: "+ NewJFrame.jProgressBar1.getValue());
}
 else jTextArea1.setText("Ответ Неверный!!!");
    }                                        
    private void jButton5ActionPerformed(java.awt.event.ActionEvent evt) {                                         
try{
    if (nomVopr>=9){
jTextArea1.setText("Эта викторина окончена! Займитесь следующей ;)");
jTextArea2.setText("Только НЕ закрывайте это окно!");
System.out.println ("123");
NewJFrame.clos=2;
        }
        nomVopr++;
show_vopr(nomVopr);
jButton1.setVisible(true);
jButton2.setVisible(true);
jButton3.setVisible(true);
jButton4.setVisible(true);

        }
catch(Exception e)
{
{
System.out.println (e);
}

    }                                        
    }
    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
jButton5.setVisible(true);
jTextArea2.setVisible(true);
jScrollPane2.setVisible(true);
jButton1.setVisible(false);
jButton2.setVisible(false);
jButton3.setVisible(false);
jButton4.setVisible(false);
        if (jButton2.getText().equals(ViktorData [nomVopr-1][2]))
 {
   jTextArea1.setText("Ответ верный!!!");
   NewJFrame.jProgressBar1.setValue(NewJFrame.jProgressBar1.getValue()+1);
   NewJFrame.jLabel1.setText("Ваш прогресс: "+ NewJFrame.jProgressBar1.getValue());
}
 else jTextArea1.setText("Ответ Неверный!!!");
    }                                        
    private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {                                         
      jButton5.setVisible(true);
jTextArea2.setVisible(true);
jScrollPane2.setVisible(true);
jButton1.setVisible(false);
jButton2.setVisible(false);
jButton3.setVisible(false);
jButton4.setVisible(false);
        if (jButton3.getText().equals(ViktorData [nomVopr-1][2]))
 {
   jTextArea1.setText("Ответ верный!!!");
  NewJFrame.jProgressBar1.setValue(NewJFrame.jProgressBar1.getValue()+1);
   NewJFrame.jLabel1.setText("Ваш прогресс: "+ NewJFrame.jProgressBar1.getValue());
}
 else jTextArea1.setText("Ответ Неверный!!!");
    }                                        
    private void jButton4ActionPerformed(java.awt.event.ActionEvent evt) {                                         
      jButton5.setVisible(true);
jTextArea2.setVisible(true);
jScrollPane2.setVisible(true);
jButton1.setVisible(false);
jButton2.setVisible(false);
jButton3.setVisible(false);
jButton4.setVisible(false);
        if (jButton4.getText().equals(ViktorData [nomVopr-1][2]))
 {
   jTextArea1.setText("Ответ верный!!!");
  NewJFrame.jProgressBar1.setValue(NewJFrame.jProgressBar1.getValue()+1);
   NewJFrame.jLabel1.setText("Ваш прогресс: "+ NewJFrame.jProgressBar1.getValue());

}
 else jTextArea1.setText("Ответ Неверный!!!");
    }                                        

    public static void main(String args[]) {
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new NewJFrame1().setVisible(true);
            }
        });
    }
    // Variables declaration - do not modify                     
    private javax.swing.JButton jButton1;
    private javax.swing.JButton jButton2;
    private javax.swing.JButton jButton3;
    private javax.swing.JButton jButton4;
    private javax.swing.JButton jButton5;
    private javax.swing.JScrollPane jScrollPane1;
    private javax.swing.JScrollPane jScrollPane2;
    private javax.swing.JTextArea jTextArea1;
    private javax.swing.JTextArea jTextArea2;
    // End of variables declaration                   
}
