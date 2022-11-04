 public class A13Complex {
    int Real, Imaginary;

    Complex() {
    }

    Complex(int Real1, int Imaginary1) {
        Real = Real1;
        Imaginary = Imaginary1;
    }

    Complex AddComplex(Complex C1, Complex C2) {
        Complex CSum = new Complex();
        CSum.Real = C1.Real + C2.Real;
        CSum.Imaginary = C1.Imaginary + C2.Imaginary;
        return CSum;
    }

    Complex subtractComplex(Complex C1, Complex C2) {
        Complex CSubtract = new Complex();
        CSubtract.Real = C1.Real - C2.Real;
        CSubtract.Imaginary = C1.Imaginary - C2.Imaginary;
        return CSubtract;
    }

    Complex MultiplyComplex(Complex C1, Complex C2) {
        Complex CMultiply = new Complex();
        CMultiply.Real = C1.Real * C2.Real;
        CMultiply.Imaginary = C1.Imaginary * C2.Imaginary;
        return CMultiply;
    }

    public static void main(String[] a) {
        Complex C1 = new Complex(6, 7);
        Complex C2 = new Complex(6, 5);
        Complex C3 = new Complex();
        Complex C4 = new Complex();
        Complex C9 = new Complex();
        C3 = C3.AddComplex(C1, C2);
        Complex C5 = new Complex(6, 7);
        Complex C6 = new Complex(6, 5);
        C4 = C4.subtractComplex(C5, C6);
        Complex C7 = new Complex(6, 7);
        Complex C8 = new Complex(6, 5);
        C9 = C9.MultiplyComplex(C7, C8);

        System.out.println("Sum:" + C3.Real + "+i" + C3.Imaginary);
        System.out.println("Subtract:" + C4.Real + "+i" + C4.Imaginary);
        System.out.println("Multiply:" + C9.Real + "+i" + C9.Imaginary);
    }
}
