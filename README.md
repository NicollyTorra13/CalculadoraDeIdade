# CalculadoraDeIdade
Calculadora de Idade JavaScript
function calculaIdade(anoNascimento, anoAtual = new Date().getFullYear()) {
  return anoNascimento <= anoAtual
    ? `Você tem ${anoAtual - anoNascimento} anos de idade.`
    : 'Mensagem de erro: Ano de nascimento é maior que o ano atual.';
}

// Exemplos de uso:
console.log(calculaIdade(1984, 2023)); // Saída: Você tem 39 anos de idade.
console.log(calculaIdade(2000, 2023)); // Saída: Você tem 23 anos de idade.
console.log(calculaIdade(2005, 1990)); // Saída: Mensagem de erro: Ano de nascimento é maior que o ano atual.
