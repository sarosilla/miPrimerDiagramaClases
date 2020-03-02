```mermaid
classDiagram

    IniciarPrograma -- "0..1" Agenda: test1
    Agenda -- "0..1" ListaEnlaza: lista
    ListaEnlaza -- "0..1" Nodo: -inicio
    Nodo "0..1" -- Nodo: enlace

Class Persona{
    - nombre: String
    - Telefono: String
    - Direccion: String
    + getNombre(): String
    + setNombre(String): void
    + getTelefono(): String
    + setTelefono(String): void
    + getDireccion(): String
    + setDireccion(String): void
}

class Agenda{
    - Agenda
    - IntroducirDatos(): Persona
    + VerLista(): void
    + listaVacia(): boolean
    + nuevaPersona(): void
    + editarPersona(): void
    + eliminarPersona(): void
    + visualizarMenu(): Integer
    + arrancarAplicacion(): void

}

Class Nodo{
    - Info: Object
}

Class ListaEnlaza{
    - insertarAlPrincipio(Object): void
    - verLista(): void
    - elementoAbuscar(): Object
    - buscar(Object): void
    - buscarContacto(Persona): Nodo
    - listaVacia(): boolean
    - insertaFinal(Object): void
    - eliminar(Object): boolean 
}

Class test{
    - test()
    - main(String[]): void
}

Class IniciarPrograma{
    - iniciarPrograma()
    - iniciarPrograma(): void
}

