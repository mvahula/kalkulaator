#impordin math
from math import sqrt
#teen klassi
class cal():

    #meetodid

    def __init__(self, a, b, c):
        self.a = a
        self.b = b
        self.c = c

    def liitmine(self):
        return self.a + self.b
    def lahutamine(self):
        return self.a - self.b
    def korrutamine(self):
        return self.a * self.b
    def jagamine(self):
        return self.a / self.b
    def jaak(self):
        return self.a % self.b
    def ruutjuur1(self):
        return sqrt(self.a)
    def ruutjuur2(self):
        return sqrt(self.b)
    def astendamine(self):
        return self.a ** self.b
    def kolmearvugaliitmine(self):
        return self.a + self.b + self.c

#objektid
a = int(input("Sisesta esimene number: "))
b = int(input("Sisesta teine number: "))
c =  int(input("Sisesta kolmas number: "))

kalk = cal(a,b,c)
while True:

    #menüüfunktsioon
    def menu():
        x = ('1. Liitmine \n2. lahutamine\n3. korrutamine\n4. jagamine\n5. Jäägi leidmine\n6. a Ruutjuure leidmine.\n7. b Ruutjuure leidmine\n8. Astendamine (a astmes b)\n9. Lisa kolmas arv ja liida kõik kokku')
        print(x)
    menu()
    valik = int(input('Sisesta üks valikutest: '))

    #if else
    if valik == 1:
        print("Vastus: ",kalk.liitmine())
        break
    elif valik == 2:
        print("Vastus: ",kalk.lahutamine())
        break
    elif valik == 3:
        print("Vastus: ",kalk.korrutamine())
        break
    elif valik == 4:
        print("Vastus: ",kalk.jagamine())
        break
    elif valik == 5:
        print("Vastus: ",kalk.jaak())
        break
    elif valik == 6:
        print("Vastus: ",kalk.ruutjuur1())
        break
    elif valik == 7:
        print("Vastus: ",kalk.ruutjuur2())
    elif valik == 8:
        print("Vastus: ",kalk.astendamine())
    elif valik == 9:
        print("Vastus: ",kalk.kolmearvugaliitmine())
    elif valik == 0:
        print('Sisesta uuesti üks liitmise operaator')
    break
