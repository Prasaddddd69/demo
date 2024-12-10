using System;

class Rectangle
{
    public double Length { get; set; }
    public double Width { get; set; }

    public double GetArea()
    {
        return Length * Width;
    }

    public double GetPerimeter()
    {
        return 2 * (Length + Width);
    }
}

class Program
{
    static void Main(string[] args)
    {
        Rectangle rect = new Rectangle();
        rect.Length = 10;
        rect.Width = 5;

        Console.WriteLine("Area: " + rect.GetArea());
        Console.WriteLine("Perimeter: " + rect.GetPerimeter());
    }
}

