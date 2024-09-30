# Java - Estudo.
<div style = "display: inline_block"><br/>
<img align="center" alt= "html5" src= "https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
<img align="center" alt= "html5" src= "https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white" />
</div><br/>


Um dos primeiros códigos que me fizeram bater cabeça rsrs:

Scanner scan = new Scanner(System.in);
		
		String vNome;
		String vSexo;
		String vEstCivil;
		int vIdade;
		double vSalario;
	
		
		while (true) {
			System.out.println("Qual seu nome?");
			vNome = scan.next();
			
			if (vNome.length() < 3 ) {
				System.out.println("Nome deve conter no mínimo 3 caracteres.");
			} else {
				
				while (true) {
					System.out.println("Qual sua idade?");
					vIdade = scan.nextInt();
					
					if (vIdade >= 0 && vIdade <= 150) {	
					 break;
					} else System.out.println("Idade inválida, digite novamente.");
				}
				while (true) {
					System.out.println("Qual seu salário?");
					vSalario = scan.nextDouble();
					
					if (vSalario > 0) {
						break;
					} else System.out.println("Salário inválido, deve ser maior que 0(zero)");
				}
				while (true) {
					System.out.println("Qual seu sexo?(M/F)");
					vSexo = scan.next().toUpperCase();
					
					if (vSexo.equals("M")  || vSexo.equals("F")) {
						break;
					} else System.out.println("Valor inválido, deve-se digitar M-Masculo ou F-Feminino");
				}
				while (true) {
					System.out.println("Qual seu Estado Civil? (S-Solteiro, C-Casado, V-Viuvo, D-Divorciado.");
					vEstCivil = scan.next().toUpperCase();
					
					if (vEstCivil.equals("S") || vEstCivil.equals("C") || vEstCivil.equals("V") || vEstCivil.equals("D")) {
						break;
					} else System.out.println("Valor inválido, deve-se definir (S-Solteiro, C-Casado, V-Viuvo, D-Divorciado).");
				}
				
				System.out.println("Após verificações validamos que: ");
				System.out.println("Seu nome é: " + vNome);
				System.out.println("Sua idade é: " + vIdade);
				System.out.println("Seu salário é: " + vSalario + " R$.");
				System.out.println("Seu sexo é: " + vSexo);
				System.out.println("Seu estado civil é: " + vEstCivil); break;
			}
		  }
