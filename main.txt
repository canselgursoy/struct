using System;
namespace struct_kavrami
{
    class Program
    {
        static void Main(string[] args)
        {
           Dikdortgen dikdörtgen = new Dikdortgen();
           dikdörtgen.Kısakenar=3;
           dikdörtgen.Uzunkenar=4;
           Console.WriteLine("class alan hesabı:{0} ",dikdörtgen.AlanHesapla());

           Dikdortgen_Struct dikdörtgen_struct = new Dikdortgen_Struct(3,4);
           
           Console.WriteLine("class alan hesabı:{0} ",dikdörtgen_struct.AlanHesapla());

        }
    }

    class Dikdortgen
    {
        public int Kısakenar;
        public int Uzunkenar;

        public Dikdortgen()
        {
            Kısakenar=3;
            Kısakenar=4;
        }

        public long AlanHesapla()
        {
            return this.Kısakenar*this.Uzunkenar;

        }
    }

    struct Dikdortgen_Struct
    {
        public int Kısakenar;
        public int Uzunkenar;

        public Dikdortgen_Struct(int kısakenar,int uzunkenar)
        {
            Kısakenar =kısakenar;
            Uzunkenar =uzunkenar;
            
        }



        public long AlanHesapla()
        {
            return this.Kısakenar*this.Uzunkenar;

        }

    }
}