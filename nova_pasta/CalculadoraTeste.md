package aula_calculadora;

import javax.swing.*;

public class CalculadoraTeste {
    public static void main(String[] args) {
        ControladorCalculadora controlador = new ControladorCalculadora();
        Calculadora2 calc = new Calculadora2(controlador);

        JFrame janela = new JFrame("calculadora");
        janela.setContentPane(calc.getPanel1());
        janela.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

        janela.pack();
        janela.setLocationRelativeTo(null);
        janela.setVisible(true);
    }
}
