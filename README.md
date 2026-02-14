# INF512-Unidad1-POO
Proyecto académico de INF512 - Unidad 1. Implementación de una clase en C# aplicando principios de Programación Orientada a Objetos como encapsulamiento y estructura de clases.
using System;

namespace INF512_Unidad1_POO
{
    class Estudiante
    {
        private string nombre;
        private string matricula;
        private string carrera;

        public Estudiante(string nombre, string matricula, string carrera)
        {
            this.nombre = nombre;
            this.matricula = matricula;
            this.carrera = carrera;
        }

        public string Nombre
        {
            get { return nombre; }
            set { nombre = value; }
        }

        public void MostrarInformacion()
        {
            Console.WriteLine("Nombre: " + nombre);
            Console.WriteLine("Matrícula: " + matricula);
            Console.WriteLine("Carrera: " + carrera);
        }

        public void Estudiar()
        {
            Console.WriteLine(nombre + " está estudiando POO.");
        }
    }
}
