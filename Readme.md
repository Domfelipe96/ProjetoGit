//Inicio da função
function processArray(arr) {
    let teste = [];
    for (let i = 0; i < arr.length; i++) {
        if (arr[i].toLowerCase().includes('a')) {
            teste.push(arr[i].toLowerCase().split('').reverse().join(''));
        } else {
            teste.push(arr[i].toUpperCase());
        }
    }
    return teste;
}
//Segue abaixo a array informada para o teste
const arr = ['BaNaNa', 'MESA', 'fogo', 'tijolo', 'caSA', 'RIO', 'Sol', 'Chave'];
//Segue abaixo a variável constante criada e a função que chama a array criada acima
const processedArr = processArray(arr);
//Segue abaixo o comando que retorna o resultado da função
console.log(processedArr);
