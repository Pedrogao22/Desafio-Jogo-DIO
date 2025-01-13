// Definição da classe Heroi
class Heroi {
    // Construtor que recebe e inicializa as propriedades nome, idade e tipo
    constructor(nome, idade, tipo) {
      this.nome = nome;
      this.idade = idade;
      this.tipo = tipo;
    }
  
    // Método atacar que exibe a mensagem de ataque baseada no tipo do herói
    atacar() {
      let ataque;
  
      // Determina o tipo de ataque com base no tipo do herói
      switch (this.tipo.toLowerCase()) {
        case 'mago':
          ataque = 'usou magia';
          break;
        case 'guerreiro':
          ataque = 'usou espada';
          break;
        case 'monge':
          ataque = 'usou artes marciais';
          break;
        case 'ninja':
          ataque = 'usou shuriken';
          break;
        default:
          ataque = 'fez um ataque genérico';
          break;
      }
  
      // Exibe a mensagem de ataque
      console.log(`O ${this.tipo} atacou usando ${ataque}`);
    }
  }
  
  // Exemplo de criação de heróis e uso do método atacar
  const mago = new Heroi('Gandalf', 1000, 'mago');
  mago.atacar(); // Saída: O mago atacou usando magia
  
  const guerreiro = new Heroi('Aragorn', 87, 'guerreiro');
  guerreiro.atacar(); // Saída: O guerreiro atacou usando espada
  
  const monge = new Heroi('Aang', 112, 'monge');
  monge.atacar(); // Saída: O monge atacou usando artes marciais
  
  const ninja = new Heroi('Naruto', 17, 'ninja');
  ninja.atacar(); // Saída: O ninja atacou usando shuriken
  
