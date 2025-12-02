function calcularSaldo(vitorias, derrotas) {
    return vitorias - derrotas;
}

function classificarNivel(vitorias) {
    if (vitorias < 10) return "Ferro";
    if (vitorias <= 20) return "Bronze";
    if (vitorias <= 50) return "Prata";
    if (vitorias <= 80) return "Ouro";
    if (vitorias <= 90) return "Diamante";
    if (vitorias <= 100) return "Lendário";
    return "Imortal";
}

let vitorias = 87;
let derrotas = 20;

let saldo = calcularSaldo(vitorias, derrotas);
let nivel = classificarNivel(vitorias);

console.log(" O Herói tem de saldo de " + saldo + " está no nível de " + nivel)
