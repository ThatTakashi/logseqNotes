- ```java
  btnTransfer.addActionListener(new ActionListener() {
  	public void actionPerformed(ActionEvent e) {
          getContentPane().removeAll();
  		setContentPane(TransferWindow.createTransferPanel());
  		getContentPane().revalidate();
  		getContentPane().repaint();
  	}
  });
  ```
-