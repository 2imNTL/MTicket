void setFont(JLabel lbl){
        try {
            Font tf = Font.createFont(Font.TRUETYPE_FONT, new File(this.getClass().getResource("/mticket/font/LeckerliOne-Regular.ttf").toURI())).deriveFont(40f); 
            lbl.setFont(tf);
        } catch (FontFormatException ex) {
            Logger.getLogger(loginForm.class.getName()).log(Level.SEVERE, null, ex);
        } catch (IOException ex) {
            Logger.getLogger(loginForm.class.getName()).log(Level.SEVERE, null, ex);
        } catch (URISyntaxException ex) {
            Logger.getLogger(loginForm.class.getName()).log(Level.SEVERE, null, ex);
        }
    }
