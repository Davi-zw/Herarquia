# Herarquia7
class funcionario:
     def __init__(self,indice,nome,login,salario):
        self.indice = indice
        self.nome = nome
        self.login = login
        self.salario = salario


     def info(self):   
         return (f"#{self.indice} - nome:  {self.nome} - email: {self.login}@empresa.com - salario: {self.salario}") 

f = funcionario(0,"Joao","Joao ",3500)
print(f.info())

class estagiario ( funcionario):
      def __init__(self,indice, nome, login, salario, ano_matricula):
         super().__init__( indice, nome, login, salario)
         self.ano_matricula = ano_matricula



class Tecnico(funcionario):
      def __init__(self, indice, nome, login, salario, nivel=1):
         super(). __init__(indice, nome, login, salario)
         self.nivel = nivel 

class Tecnico(Funcionario):
    def __init__(self, indice, nome, login, salario, nivel=1):
        super().__init__(indice, nome, login, salario)
        self.nivel = nivel




f = funcionario(0,"Joao", "Joao Talevi", 3500)
e = estagiario(1,"Daniel"," Daniel Cordeiro", 1900,2020)
g = Tecnico(2,"Gabriel","Victor Henrique", 5400,1)
h = Tecnico(3,"Rodrigo", "Rodrigo Talevi", 5400,2)


print(f.info)
print(e.info)
print(g.info)
print(h.info)
