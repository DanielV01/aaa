# aaa


package classe.executavel;



public class ClasseExecutavel {

	public static void main(String[] args) {
		
		/*
		Correntista correntista = new Correntista(1234654, 0);
		
		Conta conta = new Conta("Zezinho", 31, 234567890, 907823212, 999887766);
		
		correntista.SaldoELimite(1000.00, 500.00);
		
		/*correntista.Deposito(500.00);
		correntista.Saque(100.00);

		System.out.println(conta.toString());
		
		Double valorSaque = 200.00;
		System.out.println(correntista.Saque(valorSaque));
		
		double valorDeposito = 500.00;
		System.out.println(correntista.Deposito(valorDeposito));
		
		System.out.println(correntista.Extrato())
		*/
	}

}
package classe.modelo;

public class Conta {
	private int numeroConta;
	private Pessoa correntista;
	private double limite;
	private double saldo;
	
	public int getNumeroConta() {
		return numeroConta;
	}
	public void setNumeroConta(int numeroConta) {
		this.numeroConta = numeroConta;
	}
	public Pessoa getCorrentista() {
		return correntista;
	}
	public void setCorrentista(Pessoa correntista) {
		this.correntista = correntista;
	}
	public double getLimite() {
		return limite;
	}
	public void setLimite(double limite) {
		this.limite = limite;
	}
	public double getSaldo() {
		return saldo;
	}
	public void setSaldo(double saldo) {
		this.saldo = saldo;
	}
	
	
}
package classe.modelo;

public class ContaEspecial extends Conta {
	private float limite;
	
	public ContaEspecial() {
		
	}
	
	public ContaEspecial(int numeroConta, Pessoa correntista, double saldo, float limite) {
		super();
		this.limite = limite;		
	}

	public double getLimite() {
		return limite;
	}

	public void setLimite(float limite) {
		this.limite = limite;
	}
	
	
	
	
}
package classe.modelo;

public class ContaPoupanca extends Conta {
	
	public ContaPoupanca() {
		
	}
	
	public ContaPoupanca(int numeroConta, Pessoa correntista, double limite, double saldo) {
		super();
	}
	
	public void Juros(double juros) {
		
		this.getSaldo() + this.getSaldo() *  juros / 100;
		return;
	}
}
package classe.modelo;

public class Pessoa {
	
	private String nome;
	private long celular;
	private String email;
	
	public Pessoa() {
		
	}
	
	public Pessoa(String nome, long celular, String email) {
		this.nome = nome;
		this.celular = celular;
		this.email = email;
	}

	public String getNome() {
		return nome;
	}

	public void setNome(String nome) {
		this.nome = nome;
	}

	public long getCelular() {
		return celular;
	}

	public void setCelular(long celular) {
		this.celular = celular;
	}

	public String getEmail() {
		return email;
	}

	public void setEmail(String email) {
		this.email = email;
	}
	
	
}
