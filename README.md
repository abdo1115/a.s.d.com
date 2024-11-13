<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-9">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apprendre les Langages de Programmation</title>
    <style>
        /* Styles de base */
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #f4f7f6;
            color: #333;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        h1 {
            font-size: 3em;
            color: #2ecc71;
            margin: 50px 0;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
            font-weight: bold;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 30px;
            justify-items: center;
        }

        /* Style des cartes de langages */
        .language {
            background-color: #ffffff;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            padding: 30px;
            width: 85%;
            max-width: 280px;
            height: 1200px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 0.7s ease-out forwards;
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
            margin-bottom: 40px; /* Espacement entre les cartes */
        }
        .language:hover {
            transform: translateY(-10px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
        }
        .language h2 {
            color: #2ecc71;
            font-size: 1.7em;
            margin-bottom: 10px;
        }
        .description {
            font-size: 1.1em;
            color: #555;
            margin: 15px 0;
            line-height: 1.6;
        }
        .summary, .basics {
            color: #777;
            margin-top: 10px;
            font-size: 1em;
        }
        .btn-learn {
            display: inline-block;
            padding: 12px 25px;
            margin-top: 15px;
            font-size: 1.1em;
            font-weight: bold;
            color: #fff;
            background-color: #2ecc71;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            transition: background-color 0.3s, transform 0.3s;
        }
        .btn-learn:hover {
            background-color: #27ae60;
            transform: scale(1.05);
        }

        /* Animation d'apparition */
        @keyframes fadeInUp {
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Style des exemples de code */
        pre {
            background-color: #f4f4f4;
            padding: 15px;
            border-radius: 8px;
            font-size: 1.1em;
            color: #333;
            overflow-x: auto;
            margin-top: 10px;
            white-space: pre-wrap;
            word-wrap: break-word;
        }

        /* Section de résumé */
        .summary {
            font-size: 1em;
            color: #777;
            margin-top: 10px;
        }

        /* Réactivité */
        @media (max-width: 768px) {
            .container {
                grid-template-columns: 1fr;
                gap: 20px;
            }
        }
    </style>
</head>
<body>

    <h1>Apprendre les Langages de Programmation</h1>
    <div class="container">

        <!-- Langage 1 - JavaScript -->
        <div class="language">
            <h2>JavaScript</h2>
            <p class="description">JavaScript est utilisé pour rendre les pages web interactives et dynamiques. C'est l'un des langages les plus populaires pour le développement web.</p>
            <p class="summary"><strong>Résumé :</strong> JavaScript permet de manipuler le DOM (Document Object Model) et d’ajouter des interactions dynamiques aux sites web.</p>
            <p class="basics"><strong>Bases :</strong> Variables, fonctions, boucles, événements, et manipulation du DOM.</p>
            <pre>
// Exemple en JavaScript
let message = "Bonjour, monde!";
console.log(message);

function addition(a, b) {
    return a + b;
}
console.log(addition(2, 3));
            </pre>
            <a href="https://developer.mozilla.org/fr/docs/Web/JavaScript" target="_blank" class="btn-learn">En savoir plus</a>
        </div>

        <!-- Langage 2 - Python -->
        <div class="language">
            <h2>Python</h2>
            <p class="description">Python est un langage polyvalent et puissant, connu pour sa syntaxe claire et sa grande facilité d’utilisation. Il est utilisé dans des domaines comme l'intelligence artificielle, l’analyse de données, et le développement web.</p>
            <p class="summary"><strong>Résumé :</strong> Python est très utilisé dans la science des données, l’automatisation, et le développement d'applications web.</p>
            <p class="basics"><strong>Bases :</strong> Variables, boucles, fonctions, types de données, et gestion des erreurs.</p>
            <pre>
# Exemple en Python
message = "Bonjour, monde!"
print(message)

def addition(a, b):
    return a + b
print(addition(2, 3))
            </pre>
            <a href="https://www.python.org/" target="_blank" class="btn-learn">En savoir plus</a>
        </div>

        <!-- Langage 3 - Java -->
        <div class="language">
            <h2>Java</h2>
            <p class="description">Java est utilisé dans le développement d'applications Android, les applications d'entreprise, et pour des projets à grande échelle grâce à sa robustesse et son architecture orientée objet.</p>
            <p class="summary"><strong>Résumé :</strong> Java est fortement utilisé pour la création de systèmes d'entreprise et d’applications mobiles (Android).</p>
            <p class="basics"><strong>Bases :</strong> Classes, objets, héritage, interfaces, gestion des exceptions.</p>
            <pre>
// Exemple en Java
public class Main {
    public static void main(String[] args) {
        String message = "Bonjour, monde!";
        System.out.println(message);
        System.out.println(addition(2, 3));
    }

    public static int addition(int a, int b) {
        return a + b;
    }
}
            </pre>
            <a href="https://www.oracle.com/java/" target="_blank" class="btn-learn">En savoir plus</a>
        </div>

        <!-- Langage 4 - C# -->
        <div class="language">
            <h2>C#</h2>
            <p class="description">C# est utilisé pour développer des applications de bureau, des jeux avec Unity, et des services backend pour des sites web.</p>
            <p class="summary"><strong>Résumé :</strong> C# est un langage polyvalent, notamment utilisé pour le développement de jeux vidéo avec Unity et des applications sur le framework .NET.</p>
            <p class="basics"><strong>Bases :</strong> Classes, méthodes, objets, gestion des erreurs.</p>
            <pre>
// Exemple en C#
using System;

class Program {
    static void Main() {
        string message = "Bonjour, monde!";
        Console.WriteLine(message);

        Console.WriteLine(Addition(2, 3));
    }

    static int Addition(int a, int b) {
        return a + b;
    }
}
            </pre>
            <a href="https://learn.microsoft.com/fr-fr/dotnet/csharp/" target="_blank" class="btn-learn">En savoir plus</a>
        </div>

        <!-- Langage 5 - Ruby -->
        <div class="language">
            <h2>Ruby</h2>
            <p class="description">Ruby est un langage dynamique et orienté objet, célèbre pour sa simplicité et sa productivité. Il est couramment utilisé dans le développement web, notamment avec le framework Ruby on Rails.</p>
            <p class="summary"><strong>Résumé :</strong> Ruby est un excellent langage pour développer rapidement des applications web grâce à sa syntaxe claire et son framework Ruby on Rails.</p>
            <p class="basics"><strong>Bases :</strong> Variables, classes, méthodes, héritage, et gestion des erreurs.</p>
            <pre>
# Exemple en Ruby
message = "Bonjour, monde!"
puts message

def addition(a, b)
  return a + b
end
puts addition(2, 3)
            </pre>
            <a href="https://www.ruby-lang.org/fr/" target="_blank" class="btn-learn">En savoir plus</a>
        </div>

        <!-- Langage 6 - Swift -->
        <div class="language">
            <h2>Swift</h2>
            <p class="description">Swift est un langage de programmation moderne créé par Apple pour le développement d'applications iOS, macOS, et plus encore. Il combine des éléments de langages modernes avec une syntaxe claire et expressive.</p>
            <p class="summary"><strong>Résumé :</strong> Swift est utilisé pour développer des applications pour les plateformes Apple, offrant une sécurité de type et des performances optimisées.</p>
            <p class="basics"><strong>Bases :</strong> Variables, fonctions, classes, et gestion de la mémoire avec ARC (Automatic Reference Counting).</p>
            <pre>
// Exemple en Swift
let message = "Bonjour, monde!"
print(message)

func addition(a: Int, b: Int) -> Int {
    return a + b
}
print(addition(a: 2, b: 3))
            </pre>
            <a href="https://developer.apple.com/swift/" target="_blank" class="btn-learn">En savoir plus</a>
        </div>

        <!-- Langage 7 - Kotlin -->
        <div class="language">
            <h2>Kotlin</h2>
            <p class="description">Kotlin est un langage de programmation moderne et statiquement typé, entièrement compatible avec Java et souvent utilisé pour développer des applications Android.</p>
            <p class="summary"><strong>Résumé :</strong> Kotlin est apprécié pour sa concision, sa sécurité de type, et sa compatibilité avec Java. Il est désormais le langage préféré pour le développement Android.</p>
            <p class="basics"><strong>Bases :</strong> Variables, fonctions, classes, et lambdas.</p>
            <pre>
// Exemple en Kotlin
fun main() {
    val message = "Bonjour, monde!"
    println(message)

    fun addition(a: Int, b: Int): Int {
        return a + b
    }
    println(addition(2, 3))
}
            </pre>
            <a href="https://kotlinlang.org/" target="_blank" class="btn-learn">En savoir plus</a>
        </div>

        <!-- Langage 8 - Go -->
        <div class="language">
            <h2>Go</h2>
            <p class="description">Go, aussi appelé Golang, est un langage créé par Google, conçu pour être simple, rapide, et efficace pour le développement de systèmes et d'applications distribuées.</p>
            <p class="summary"><strong>Résumé :</strong> Go est idéal pour les applications backend, le développement de microservices, et les systèmes distribués grâce à sa simplicité et ses performances.</p>
            <p class="basics"><strong>Bases :</strong> Variables, fonctions, goroutines, et gestion de la concurrence.</p>
            <pre>
// Exemple en Go
package main
import "fmt"

func main() {
    message := "Bonjour, monde!"
    fmt.Println(message)

    fmt.Println(addition(2, 3))
}

func addition(a, b int) int {
    return a + b
}
            </pre>
            <a href="https://golang.org/" target="_blank" class="btn-learn">En savoir plus</a>
        </div>

    </div>
</body>
</html>
