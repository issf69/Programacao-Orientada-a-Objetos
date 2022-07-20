# Programacao-Orientada-a-Objetos
Exercícios Programação Orientada a Objetos
## package dio.me;

/**
 * Classe de exemplo para o exercício da Aula 2 de Orientação a Objetos.
 */

public class Carro {
    String cor;
    String modelo;
    int capacidadeTanque;

    Carro() {

    }

    Carro(String cor, String modelo, int capacidadeTanque) {
        this.cor = cor;
        this.modelo = modelo;
        this.capacidadeTanque = capacidadeTanque;
    }

    void setCor(String cor) {
        this.cor = cor;
    }

    String getCor() {
        return cor;
    }

    void setModelo(String modelo) {
        this.modelo = modelo;
    }

    String getModelo() {
        return modelo;
    }

    void setCapacidadeTanque(int capacidadeTanque) {
        this.capacidadeTanque = capacidadeTanque;
    }

    int getCapacidadeTanque() {
        return capacidadeTanque;
    }

    double totalValorTanque(double valorCombustivel) {
        return capacidadeTanque * valorCombustivel;
    }
}

### package dio.me;

/**
 *
 */
public class RodarAplicacao {
    public static void main(String[] args) {
        Carro carro1 = new Carro();

        carro1.setCor("Azul");
        carro1.setModelo("BMW Serie 3");
        carro1.setCapacidadeTanque(59);

        System.out.println(carro1.getModelo());
        System.out.println(carro1.getCor());
        System.out.println(carro1.getCapacidadeTanque());
        System.out.println(carro1.totalValorTanque(6.39));

        Carro carro2 = new Carro("Cinza", "Mercedes-Benz Classe C ", 66);

        System.out.println(carro2.getModelo());
        System.out.println(carro2.getCor());
        System.out.println(carro2.getCapacidadeTanque());
        System.out.println(carro2.totalValorTanque(6.46));

    }
}

#### C:\Users\Irene\.jdks\openjdk-18.0.1.1\bin\java.exe "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.1.1\lib\idea_rt.jar=55813:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.1.1\bin" -Dfile.encoding=UTF-8 -classpath "C:\Users\Irene\Documents\Orientacao Objetos-Sepro prof Tiago\orientacao-objetos\out\production\orientacao-objetos" dio.me.RodarAplicacao
BMW Serie 3
Azul
59
377.01
Mercedes-Benz Classe C 
Cinza
66
426.36

Process finished with exit code 0
