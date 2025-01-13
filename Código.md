# cadastrodeusuariopython.github.io
Cadastro de Usuário em Python
class Usuario:
    def __init__(self, nome_completo, nacionalidade, profissao, estado_civil, cpf, endereco, email, telefone):
        self.nome_completo = nome_completo
        self.nacionalidade = nacionalidade
        self.profissao = profissao
        self.estado_civil = estado_civil
        self.cpf = cpf
        self.endereco = endereco
        self.email = email
        self.telefone = telefone

    def __str__(self):
        return (f"Nome Completo: {self.nome_completo}\n"
                f"Nacionalidade: {self.nacionalidade}\n"
                f"Profissão: {self.profissao}\n"
                f"Estado Civil: {self.estado_civil}\n"
                f"CPF: {self.cpf}\n"
                f"Endereço: {self.endereco}\n"
                f"E-mail: {self.email}\n"
                f"Telefone: {self.telefone}")

def main():
    print("Cadastro de Usuário")

    nome_completo = input("Digite seu nome completo: ")
    nacionalidade = input("Digite sua nacionalidade: ")
    profissao = input("Digite sua profissão: ")
    estado_civil = input("Digite seu estado civil: ")
    cpf = input("Digite seu CPF: ")
    endereco = input("Digite seu endereço: ")
    email = input("Digite seu e-mail: ")
    telefone = input("Digite seu telefone/WhatsApp: ")

    usuario = Usuario(nome_completo, nacionalidade, profissao, estado_civil, cpf, endereco, email, telefone)

    print("\nCadastro concluído com sucesso!")
    print(usuario)

if __name__ == "__main__":
    main()
