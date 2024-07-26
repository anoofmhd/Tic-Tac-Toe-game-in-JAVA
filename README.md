# Tic-Tac-Toe-game-in-JAVA
This is a Tic Tac Toe game in java. It is an modified version of the game.

import java.awt.Color;
import javax.swing.JFrame;
import javax.swing.JOptionPane;


 
    public class tic_tac_toe extends javax.swing.JFrame {
    
    private String startGame = "X";
    private int xCount = 0;
    private int oCount = 0;
    boolean checker;
    private Object JOptionpane;

    /**
     * Creates new form tic_tac_toe_frame
     */
    public tic_tac_toe() {
        initComponents();
    }

    
    private void gameScore()
    {
        jLblplayerx.setText(String.valueOf(xCount));
        jLblplayero.setText(String.valueOf(oCount));
    }
    
    private void choose_a_player(){
        if(startGame.equalsIgnoreCase("X"))
        {
            startGame = "0";
        }
        else
        {
            startGame = "X";
        }
            
    }
    private void winningGame()
    {
        String b1 = jbtnTic1.getText();
        String b2 = jbtnTic1.getText();
        String b3 = jbtnTic1.getText();
        String b4 = jbtnTic1.getText();
        String b5 = jbtnTic1.getText();
        String b6 = jbtnTic1.getText();
        String b7 = jbtnTic1.getText();
        String b8 = jbtnTic1.getText();
        String b9 = jbtnTic1.getText();
        
        if(b1 == ("X") && b2 == ("X") && b3 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Player x wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic1.setBackground(Color.ORANGE);
            jbtnTic2.setBackground(Color.ORANGE);
            jbtnTic3.setBackground(Color.ORANGE);
            xCount++;
            gameScore();
            
        }
        
        if(b4 == ("X") && b5 == ("X") && b6 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Player x wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic4.setBackground(Color.CYAN);
            jbtnTic5.setBackground(Color.CYAN);
            jbtnTic6.setBackground(Color.CYAN);
            xCount++;
            gameScore();
            
        }
         
           if(b7 == ("X") && b8 == ("X") && b9 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Player x wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic7.setBackground(Color.CYAN);
            jbtnTic5.setBackground(Color.CYAN);
            jbtnTic9.setBackground(Color.CYAN);
            xCount++;
            gameScore();
            
        }
            if(b1 == ("O") && b2 == ("0") && b3 == ("0"))
        {
            JOptionPane.showMessageDialog(this,"Player o wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic1.setBackground(Color.GREEN);
            jbtnTic2.setBackground(Color.GREEN);
            jbtnTic3.setBackground(Color.GREEN);
            oCount++;
            gameScore();
            
        }
         if(b4 == ("O") && b5 == ("O") && b6 == ("0"))
        {
            JOptionPane.showMessageDialog(this,"Player o wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic4.setBackground(Color.CYAN);
            jbtnTic5.setBackground(Color.CYAN);
            jbtnTic6.setBackground(Color.CYAN);
            oCount++;
            gameScore();
            
        }
            if(b7 == ("O") && b8 == ("O") && b9 == ("0"))
        {
            JOptionPane.showMessageDialog(this,"Player o wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic7.setBackground(Color.CYAN);
            jbtnTic8.setBackground(Color.CYAN);
            jbtnTic9.setBackground(Color.CYAN);
            oCount++;
            gameScore();
            
        }
         if(b1 == ("X") && b4 == ("X") && b7 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Player x wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic1.setBackground(Color.ORANGE);
            jbtnTic4.setBackground(Color.ORANGE);
            jbtnTic7.setBackground(Color.ORANGE);
            xCount++;
            gameScore();
            
        }
          if(b2 == ("X") && b5 == ("X") && b8 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Player x wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic2.setBackground(Color.ORANGE);
            jbtnTic5.setBackground(Color.ORANGE);
            jbtnTic8.setBackground(Color.ORANGE);
            xCount++;
            gameScore();
            
        }
           if(b3 == ("X") && b6 == ("X") && b9 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Player x wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic3.setBackground(Color.ORANGE);
            jbtnTic6.setBackground(Color.ORANGE);
            jbtnTic9.setBackground(Color.ORANGE);
            xCount++;
            gameScore();
            
        }
        if(b1 == ("O") && b4 == ("0") && b7 == ("0"))
        {
            JOptionPane.showMessageDialog(this,"Player o wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic1.setBackground(Color.GREEN);
            jbtnTic4.setBackground(Color.GREEN);
            jbtnTic7.setBackground(Color.GREEN);
            oCount++;
            gameScore();
            
        }
        if(b2 == ("O") && b5 == ("0") && b8 == ("0"))
        {
            JOptionPane.showMessageDialog(this,"Player o wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic2.setBackground(Color.GREEN);
            jbtnTic5.setBackground(Color.GREEN);
            jbtnTic8.setBackground(Color.GREEN);
            oCount++;
            gameScore();
            
        }
            if(b3 == ("O") && b6 == ("0") && b9 == ("0"))
        {
            JOptionPane.showMessageDialog(this,"Player o wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic3.setBackground(Color.GREEN);
            jbtnTic6.setBackground(Color.GREEN);
            jbtnTic9.setBackground(Color.GREEN);
            oCount++;
            gameScore();
            
        }
         if(b1 == ("X") && b5 == ("X") && b9 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Player x wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic1.setBackground(Color.ORANGE);
            jbtnTic5.setBackground(Color.ORANGE);
            jbtnTic9.setBackground(Color.ORANGE);
            xCount++;
            gameScore();
            
        }
         if(b3 == ("X") && b5 == ("X") && b7 == ("X"))
        {
            JOptionPane.showMessageDialog(this,"Player x wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic1.setBackground(Color.ORANGE);
            jbtnTic2.setBackground(Color.ORANGE);
            jbtnTic3.setBackground(Color.ORANGE);
            xCount++;
            gameScore();
            
        }
            if(b1 == ("O") && b5 == ("0") && b9 == ("0"))
        {
            JOptionPane.showMessageDialog(this,"Player o wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic1.setBackground(Color.GREEN);
            jbtnTic5.setBackground(Color.GREEN);
            jbtnTic9.setBackground(Color.GREEN);
            oCount++;
            gameScore();
            
        }
            if(b3 == ("O") && b5 == ("0") && b7 == ("0"))
        {
            JOptionPane.showMessageDialog(this,"Player o wins","Tic Tac Toe", JOptionPane.INFORMATION_MESSAGE);
            jbtnTic3.setBackground(Color.GREEN);
            jbtnTic5.setBackground(Color.GREEN);
            jbtnTic7.setBackground(Color.GREEN);
            oCount++;
            gameScore();
            
        }
         
    }
    
    /**
     * This method is called from within the constructor to initialize the form.
     * WARNING: Do NOT modify this code. The content of this method is always
     * regenerated by the Form Editor.
     */
    @SuppressWarnings("unchecked")
    private JFrame frame;
     
        
    
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        jPanel2 = new javax.swing.JPanel();
        jPanel3 = new javax.swing.JPanel();
        jPanel4 = new javax.swing.JPanel();
        query1 = java.beans.Beans.isDesignTime() ? null : ((javax.persistence.EntityManager)null).createQuery("");
        query2 = java.beans.Beans.isDesignTime() ? null : ((javax.persistence.EntityManager)null).createQuery("");
        jPanel1 = new javax.swing.JPanel();
        jPanel6 = new javax.swing.JPanel();
        jbtnTic6 = new javax.swing.JButton();
        jbtnTic1 = new javax.swing.JButton();
        jbtnTic2 = new javax.swing.JButton();
        jbtnTic3 = new javax.swing.JButton();
        jbtnTic5 = new javax.swing.JButton();
        jbtnTic4 = new javax.swing.JButton();
        jbtnTic7 = new javax.swing.JButton();
        jbtnTic8 = new javax.swing.JButton();
        jbtnTic9 = new javax.swing.JButton();
        jPanel8 = new javax.swing.JPanel();
        jPanel5 = new javax.swing.JPanel();
        jPanel7 = new javax.swing.JPanel();
        jButton = new javax.swing.JButton();
        jbtnReset = new javax.swing.JButton();
        jexitbutton = new javax.swing.JButton();
        jPanel10 = new javax.swing.JPanel();
        jPanel11 = new javax.swing.JPanel();
        jPanel12 = new javax.swing.JPanel();
        jLblplayero = new javax.swing.JLabel();
        jLabel3 = new javax.swing.JLabel();
        jLblplayerx = new javax.swing.JLabel();
        jLabel4 = new javax.swing.JLabel();
        jPanel13 = new javax.swing.JPanel();
        jPanel15 = new javax.swing.JPanel();
        jLabel2 = new javax.swing.JLabel();

        jPanel2.setBackground(new java.awt.Color(95, 158, 60));
        jPanel2.setToolTipText("");
        jPanel2.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        jPanel3.setBackground(new java.awt.Color(95, 158, 60));
        jPanel3.setToolTipText("");
        jPanel3.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        jPanel4.setBackground(new java.awt.Color(95, 158, 60));
        jPanel4.setToolTipText("");
        jPanel4.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
        setCursor(new java.awt.Cursor(java.awt.Cursor.DEFAULT_CURSOR));
        setResizable(false);
        getContentPane().setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        jPanel1.setBackground(new java.awt.Color(95, 158, 60));
        jPanel1.setToolTipText("");
        jPanel1.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        jPanel6.setBackground(new java.awt.Color(95, 158, 60));
        jPanel6.setBorder(javax.swing.BorderFactory.createBevelBorder(javax.swing.border.BevelBorder.LOWERED));
        jPanel6.setToolTipText("");
        jPanel6.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        jbtnTic6.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnTic6.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnTic6.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnTic6.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnTic6.setRequestFocusEnabled(false);
        jbtnTic6.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnTic6ActionPerformed(evt);
            }
        });
        jPanel6.add(jbtnTic6, new org.netbeans.lib.awtextra.AbsoluteConstraints(430, 140, 190, 120));

        jbtnTic1.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnTic1.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnTic1.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnTic1.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnTic1.setRequestFocusEnabled(false);
        jbtnTic1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnTic1ActionPerformed(evt);
            }
        });
        jPanel6.add(jbtnTic1, new org.netbeans.lib.awtextra.AbsoluteConstraints(30, 20, 180, 110));

        jbtnTic2.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnTic2.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnTic2.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnTic2.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnTic2.setRequestFocusEnabled(false);
        jbtnTic2.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnTic2ActionPerformed(evt);
            }
        });
        jPanel6.add(jbtnTic2, new org.netbeans.lib.awtextra.AbsoluteConstraints(220, 20, 200, 110));

        jbtnTic3.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnTic3.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnTic3.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnTic3.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnTic3.setRequestFocusEnabled(false);
        jbtnTic3.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnTic3ActionPerformed(evt);
            }
        });
        jPanel6.add(jbtnTic3, new org.netbeans.lib.awtextra.AbsoluteConstraints(430, 20, 190, 110));

        jbtnTic5.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnTic5.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnTic5.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnTic5.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnTic5.setRequestFocusEnabled(false);
        jbtnTic5.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnTic5ActionPerformed(evt);
            }
        });
        jPanel6.add(jbtnTic5, new org.netbeans.lib.awtextra.AbsoluteConstraints(220, 140, 200, 120));

        jbtnTic4.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnTic4.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnTic4.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnTic4.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnTic4.setRequestFocusEnabled(false);
        jbtnTic4.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnTic4ActionPerformed(evt);
            }
        });
        jPanel6.add(jbtnTic4, new org.netbeans.lib.awtextra.AbsoluteConstraints(30, 140, 180, 120));

        jbtnTic7.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnTic7.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnTic7.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnTic7.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnTic7.setRequestFocusEnabled(false);
        jbtnTic7.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnTic7ActionPerformed(evt);
            }
        });
        jPanel6.add(jbtnTic7, new org.netbeans.lib.awtextra.AbsoluteConstraints(30, 270, 180, 120));

        jbtnTic8.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnTic8.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnTic8.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnTic8.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnTic8.setRequestFocusEnabled(false);
        jbtnTic8.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnTic8ActionPerformed(evt);
            }
        });
        jPanel6.add(jbtnTic8, new org.netbeans.lib.awtextra.AbsoluteConstraints(220, 270, 200, 120));

        jbtnTic9.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnTic9.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnTic9.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnTic9.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnTic9.setRequestFocusEnabled(false);
        jbtnTic9.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnTic9ActionPerformed(evt);
            }
        });
        jPanel6.add(jbtnTic9, new org.netbeans.lib.awtextra.AbsoluteConstraints(430, 270, 190, 120));

        jPanel1.add(jPanel6, new org.netbeans.lib.awtextra.AbsoluteConstraints(30, 170, 650, 410));

        jPanel8.setBackground(new java.awt.Color(95, 158, 60));
        jPanel8.setBorder(javax.swing.BorderFactory.createBevelBorder(javax.swing.border.BevelBorder.LOWERED));
        jPanel8.setToolTipText("");
        jPanel8.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        jPanel5.setBackground(new java.awt.Color(95, 158, 60));
        jPanel5.setBorder(javax.swing.BorderFactory.createBevelBorder(javax.swing.border.BevelBorder.LOWERED));
        jPanel5.setToolTipText("");
        jPanel5.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        jPanel7.setBackground(new java.awt.Color(95, 158, 60));
        jPanel7.setBorder(javax.swing.BorderFactory.createBevelBorder(javax.swing.border.BevelBorder.LOWERED));
        jPanel7.setToolTipText("");
        jPanel7.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());
        jPanel5.add(jPanel7, new org.netbeans.lib.awtextra.AbsoluteConstraints(710, 20, 680, 560));

        jButton.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jButton.setText("New Game");
        jButton.setMaximumSize(new java.awt.Dimension(200, 158));
        jButton.setMinimumSize(new java.awt.Dimension(200, 158));
        jButton.setPreferredSize(new java.awt.Dimension(200, 158));
        jButton.setRequestFocusEnabled(false);
        jButton.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jButtonActionPerformed(evt);
            }
        });
        jPanel5.add(jButton, new org.netbeans.lib.awtextra.AbsoluteConstraints(10, 10, 630, 90));

        jbtnReset.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jbtnReset.setText("Reset");
        jbtnReset.setMaximumSize(new java.awt.Dimension(200, 158));
        jbtnReset.setMinimumSize(new java.awt.Dimension(200, 158));
        jbtnReset.setPreferredSize(new java.awt.Dimension(200, 158));
        jbtnReset.setRequestFocusEnabled(false);
        jbtnReset.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jbtnResetActionPerformed(evt);
            }
        });
        jPanel5.add(jbtnReset, new org.netbeans.lib.awtextra.AbsoluteConstraints(10, 110, 320, 90));

        jexitbutton.setFont(new java.awt.Font("Tahoma", 1, 96)); // NOI18N
        jexitbutton.setText("Exit");
        jexitbutton.setMaximumSize(new java.awt.Dimension(200, 158));
        jexitbutton.setMinimumSize(new java.awt.Dimension(200, 158));
        jexitbutton.setPreferredSize(new java.awt.Dimension(200, 158));
        jexitbutton.setRequestFocusEnabled(false);
        jexitbutton.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jexitbuttonActionPerformed(evt);
            }
        });
        jPanel5.add(jexitbutton, new org.netbeans.lib.awtextra.AbsoluteConstraints(350, 110, 290, 90));

        jPanel8.add(jPanel5, new org.netbeans.lib.awtextra.AbsoluteConstraints(10, 200, 660, 210));

        jPanel10.setBackground(new java.awt.Color(95, 158, 60));
        jPanel10.setBorder(javax.swing.BorderFactory.createBevelBorder(javax.swing.border.BevelBorder.LOWERED));
        jPanel10.setToolTipText("");
        jPanel10.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        jPanel11.setBackground(new java.awt.Color(95, 158, 60));
        jPanel11.setBorder(javax.swing.BorderFactory.createBevelBorder(javax.swing.border.BevelBorder.LOWERED));
        jPanel11.setToolTipText("");
        jPanel11.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());
        jPanel10.add(jPanel11, new org.netbeans.lib.awtextra.AbsoluteConstraints(710, 20, 680, 560));

        jPanel12.setBackground(new java.awt.Color(95, 158, 60));
        jPanel12.setBorder(javax.swing.BorderFactory.createBevelBorder(javax.swing.border.BevelBorder.LOWERED));
        jPanel12.setToolTipText("");
        jPanel12.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());
        jPanel10.add(jPanel12, new org.netbeans.lib.awtextra.AbsoluteConstraints(10, 180, 670, 400));

        jLblplayero.setFont(new java.awt.Font("Tahoma", 1, 66)); // NOI18N
        jLblplayero.setHorizontalAlignment(javax.swing.SwingConstants.CENTER);
        jLblplayero.setText("0");
        jLblplayero.setOpaque(true);
        jPanel10.add(jLblplayero, new org.netbeans.lib.awtextra.AbsoluteConstraints(320, 100, 300, 60));

        jLabel3.setFont(new java.awt.Font("Tahoma", 1, 66)); // NOI18N
        jLabel3.setText("Player O:");
        jPanel10.add(jLabel3, new org.netbeans.lib.awtextra.AbsoluteConstraints(10, 80, -1, -1));

        jLblplayerx.setFont(new java.awt.Font("Tahoma", 1, 66)); // NOI18N
        jLblplayerx.setHorizontalAlignment(javax.swing.SwingConstants.CENTER);
        jLblplayerx.setText("0");
        jLblplayerx.setOpaque(true);
        jPanel10.add(jLblplayerx, new org.netbeans.lib.awtextra.AbsoluteConstraints(320, 20, 300, 70));

        jLabel4.setFont(new java.awt.Font("Tahoma", 1, 66)); // NOI18N
        jLabel4.setText("Player X:");
        jPanel10.add(jLabel4, new org.netbeans.lib.awtextra.AbsoluteConstraints(10, 10, -1, -1));

        jPanel8.add(jPanel10, new org.netbeans.lib.awtextra.AbsoluteConstraints(20, 20, 640, 170));

        jPanel1.add(jPanel8, new org.netbeans.lib.awtextra.AbsoluteConstraints(700, 170, 680, 410));

        jPanel13.setBackground(new java.awt.Color(95, 158, 60));
        jPanel13.setBorder(javax.swing.BorderFactory.createBevelBorder(javax.swing.border.BevelBorder.LOWERED));
        jPanel13.setToolTipText("");
        jPanel13.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        jPanel15.setBackground(new java.awt.Color(95, 158, 60));
        jPanel15.setBorder(javax.swing.BorderFactory.createBevelBorder(javax.swing.border.BevelBorder.LOWERED));
        jPanel15.setToolTipText("");
        jPanel15.setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());
        jPanel13.add(jPanel15, new org.netbeans.lib.awtextra.AbsoluteConstraints(10, 180, 670, 400));

        jLabel2.setFont(new java.awt.Font("Verdana", 1, 66)); // NOI18N
        jLabel2.setForeground(new java.awt.Color(255, 255, 255));
        jLabel2.setText("TIC TAC TOE GAME");
        jPanel13.add(jLabel2, new org.netbeans.lib.awtextra.AbsoluteConstraints(320, 20, 720, -1));

        jPanel1.add(jPanel13, new org.netbeans.lib.awtextra.AbsoluteConstraints(20, 20, 1360, 120));

        getContentPane().add(jPanel1, new org.netbeans.lib.awtextra.AbsoluteConstraints(0, 0, 1410, 600));

        pack();
        setLocationRelativeTo(null);
    }// </editor-fold>                        

    private void jbtnTic6ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
         jbtnTic6.setText(startGame);
        
        if(startGame.equalsIgnoreCase("X"))
        {
            checker =  false;
        }
        else
        {
            checker = true;
        }
        choose_a_player();
        winningGame();
    }                                        

    private void jbtnTic8ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
         jbtnTic8.setText(startGame);
        
        if(startGame.equalsIgnoreCase("X"))
        {
            checker =  false;
        }
        else
        {
            checker = true;
        }
        choose_a_player();
        winningGame();
    }                                        

    private void jbtnTic5ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
         jbtnTic5.setText(startGame);
        
        if(startGame.equalsIgnoreCase("X"))
        {
            checker =  false;
        }
        else
        {
            checker = true;
        }
        choose_a_player();
        winningGame();
    }                                        

    private void jbtnTic2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
         jbtnTic2.setText(startGame);
        
        if(startGame.equalsIgnoreCase("X"))
        {
            checker =  false;
        }
        else
        {
            checker = true;
        }
        choose_a_player();
        winningGame();
           
    }                                        

    private void jbtnTic7ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
         jbtnTic7.setText(startGame);
        
        if(startGame.equalsIgnoreCase("X"))
        {
            checker =  false;
        }
        else
        {
            checker = true;
        }
        choose_a_player();
        winningGame();
    }                                        

    private void jbtnResetActionPerformed(java.awt.event.ActionEvent evt) {                                          
           jbtnTic1.setEnabled(true);
           jbtnTic2.setEnabled(true);
           jbtnTic3.setEnabled(true);
           jbtnTic4.setEnabled(true);
           jbtnTic5.setEnabled(true);
           jbtnTic6.setEnabled(true);
           jbtnTic7.setEnabled(true);
           jbtnTic8.setEnabled(true);
           jbtnTic9.setEnabled(true);
           
           
           
           jbtnTic1.setText("");
           jbtnTic2.setText("");
           jbtnTic3.setText("");
           jbtnTic4.setText("");
           jbtnTic5.setText("");
           jbtnTic6.setText("");
           jbtnTic7.setText("");
           jbtnTic8.setText("");
           jbtnTic9.setText("");
           
           jbtnTic1.setBackground(Color.LIGHT_GRAY);
           jbtnTic2.setBackground(Color.LIGHT_GRAY);
           jbtnTic3.setBackground(Color.LIGHT_GRAY);
           jbtnTic4.setBackground(Color.LIGHT_GRAY);
           jbtnTic5.setBackground(Color.LIGHT_GRAY);
           jbtnTic6.setBackground(Color.LIGHT_GRAY);
           jbtnTic7.setBackground(Color.LIGHT_GRAY);
           jbtnTic8.setBackground(Color.LIGHT_GRAY);
           jbtnTic9.setBackground(Color.LIGHT_GRAY);
    }                                         

    private void jexitbuttonActionPerformed(java.awt.event.ActionEvent evt) {                                            
        // TODO add your handling code here:
        frame = new JFrame("Exit");
        if(JOptionPane.showConfirmDialog(frame,"Confirm if you want to exit.","Tic Tac Toe",JOptionPane.YES_NO_OPTION)== JOptionPane.YES_NO_OPTION)
        {
            System.exit(0);
        }
    }                                           

    private void jButtonActionPerformed(java.awt.event.ActionEvent evt) {                                        
         jbtnTic1.setEnabled(true);
           jbtnTic2.setEnabled(true);
           jbtnTic3.setEnabled(true);
           jbtnTic4.setEnabled(true);
           jbtnTic5.setEnabled(true);
           jbtnTic6.setEnabled(true);
           jbtnTic7.setEnabled(true);
           jbtnTic8.setEnabled(true);
           jbtnTic9.setEnabled(true);
           
           jLblplayerx.setText("0");
           jLblplayero.setText("0");
           
           jbtnTic1.setText("");
           jbtnTic2.setText("");
           jbtnTic3.setText("");
           jbtnTic4.setText("");
           jbtnTic5.setText("");
           jbtnTic6.setText("");
           jbtnTic7.setText("");
           jbtnTic8.setText("");
           jbtnTic9.setText("");
           
           jbtnTic1.setBackground(Color.LIGHT_GRAY);
           jbtnTic2.setBackground(Color.LIGHT_GRAY);
           jbtnTic3.setBackground(Color.LIGHT_GRAY);
           jbtnTic4.setBackground(Color.LIGHT_GRAY);
           jbtnTic5.setBackground(Color.LIGHT_GRAY);
           jbtnTic6.setBackground(Color.LIGHT_GRAY);
           jbtnTic7.setBackground(Color.LIGHT_GRAY);
           jbtnTic8.setBackground(Color.LIGHT_GRAY);
           jbtnTic9.setBackground(Color.LIGHT_GRAY);
    }                                       

    private void jbtnTic1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        jbtnTic1.setText(startGame);
        
        if(startGame.equalsIgnoreCase("X"))
        {
            checker =  false;
        }
        else
        {
            checker = true;
        }
        choose_a_player();
        winningGame();
    }                                        

    private void jbtnTic3ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
         jbtnTic3.setText(startGame);
        
        if(startGame.equalsIgnoreCase("X"))
        {
            checker =  false;
        }
        else
        {
            checker = true;
        }
        choose_a_player();
        winningGame();
            
    }                                        

    private void jbtnTic4ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
         jbtnTic4.setText(startGame);
        
        if(startGame.equalsIgnoreCase("X"))
        {
            checker =  false;
        }
        else
        {
            checker = true;
        }
        choose_a_player();
        winningGame();
            
    }                                        

    private void jbtnTic9ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
         jbtnTic9.setText(startGame);
        
        if(startGame.equalsIgnoreCase("X"))
        {
            checker =  false;
        }
        else
        {
            checker = true;
        }
        choose_a_player();
        winningGame();
    }                                        

    /**
     * @param args the command line arguments
     */
    public static void main(String args[]) {
        /* Set the Nimbus look and feel */
        //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code (optional) ">
        /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
         * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
         */
        try {
            for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                if ("Nimbus".equals(info.getName())) {
                    javax.swing.UIManager.setLookAndFeel(info.getClassName());
                    break;
                }
            }
        } catch (ClassNotFoundException ex) {
            java.util.logging.Logger.getLogger(tic_tac_toe_frame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(tic_tac_toe_frame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(tic_tac_toe_frame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(tic_tac_toe_frame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(() -> {
            new tic_tac_toe_frame().setVisible(true);
        });
    }

    // Variables declaration - do not modify                     
    private javax.swing.JButton jButton;
    private javax.swing.JLabel jLabel2;
    private javax.swing.JLabel jLabel3;
    private javax.swing.JLabel jLabel4;
    private javax.swing.JLabel jLblplayero;
    private javax.swing.JLabel jLblplayerx;
    private javax.swing.JPanel jPanel1;
    private javax.swing.JPanel jPanel10;
    private javax.swing.JPanel jPanel11;
    private javax.swing.JPanel jPanel12;
    private javax.swing.JPanel jPanel13;
    private javax.swing.JPanel jPanel15;
    private javax.swing.JPanel jPanel2;
    private javax.swing.JPanel jPanel3;
    private javax.swing.JPanel jPanel4;
    private javax.swing.JPanel jPanel5;
    private javax.swing.JPanel jPanel6;
    private javax.swing.JPanel jPanel7;
    private javax.swing.JPanel jPanel8;
    private javax.swing.JButton jbtnReset;
    private javax.swing.JButton jbtnTic1;
    private javax.swing.JButton jbtnTic2;
    private javax.swing.JButton jbtnTic3;
    private javax.swing.JButton jbtnTic4;
    private javax.swing.JButton jbtnTic5;
    private javax.swing.JButton jbtnTic6;
    private javax.swing.JButton jbtnTic7;
    private javax.swing.JButton jbtnTic8;
    private javax.swing.JButton jbtnTic9;
    private javax.swing.JButton jexitbutton;
    private javax.persistence.Query query1;
    private javax.persistence.Query query2;
    // End of variables declaration                   

   
}
