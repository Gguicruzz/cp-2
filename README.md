🧠 Checkpoint 2 – Criptografia Clássica em JavaScript

Curso: Engenharia de Software
Disciplina: Web Development
Professor: Marcelo Amorim
Semestre: 2025/2

🎯 Objetivo

Implementar quatro cifras históricas da criptografia utilizando JavaScript puro (Vanilla JS), aplicando conhecimentos sobre funções, laços de repetição, manipulação de strings e aritmética modular.

🧩 Funcionalidades Implementadas
1. 🔁 Cifra Atbash

Substitui cada letra pela sua oposta no alfabeto:
A ↔ Z, B ↔ Y, C ↔ X, etc.

A codificação e decodificação são iguais.

2. 🔄 Cifra de César

Desloca cada letra do alfabeto por uma quantidade fixa (a “chave”).

Exemplo: com chave = 3 → A → D, B → E, C → F

3. 🧮 Cifra de Vigenère

Usa uma palavra-chave para aplicar deslocamentos variáveis (baseados na Cifra de César), repetindo a chave de forma cíclica.

Suporta modos codificar e decodificar.

4. 🔐 Criptografia RSA (Didática)

Simula a criptografia de chave pública e privada, utilizando números primos pequenos para fins de aprendizado.

Inclui geração de chaves e fórmulas de cifragem/decifragem com mod.

🧠 Tecnologias Utilizadas

HTML5

JavaScript (Vanilla JS)

CSS3 (opcional para estilo)

🧪 Testes de Validação
// Atbash
console.log(cifrarAtbash("OlaMundo")); 

// César
console.log(cifrarCesar("criptografia", 3)); 
console.log(cifrarCesar("fulswrjudiia", -3)); 

// Vigenère
const chaveV = "CHAVE";
const codificadoV = cifrarVigenere("Enigma!", chaveV, 'codificar');
console.log(cifrarVigenere(codificadoV, chaveV, 'decodificar'));

// RSA
const PRIMO_1 = 17;
const PRIMO_2 = 19;
const CHAVES = gerarChavesRSA_Didaticas(PRIMO_1, PRIMO_2);
const textoOriginal = "OLA";
const cifrado = cifrarRSA_Didatico(textoOriginal, CHAVES.publica.E, CHAVES.publica.N);
const decifrado = decifrarRSA_Didatico(cifrado, CHAVES.privada.D, CHAVES.privada.N);
console.log("RSA Decifrado:", decifrado);

👥 Integrantes do Grupo
Nome Guilherme cruz alves	RA 566861
	
	
	
	


📦 Estrutura do Projeto
📁 Projeto-Criptografia
├── index.html        # Interface e código principal das cifras
├── README.md         # Descrição e informações do projeto
