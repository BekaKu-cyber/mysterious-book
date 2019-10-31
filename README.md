# mysterious-book
class Creature:



    work = "Worker"
    salary = 40000


    def show(self):
        print("это работник, его", self.salary, "стольков месяц")

    def __del__(self):
        print ('деструктор')


class Driver(Creature):

    def __init__(self):
        self.work = "driver"
        self.salary = 400

    def show(self):
        print("это , его", self.work, "работа")

obj_worker = Creature()
obj_driver = Driver()
obj_worker.work()
obj_driver.work()


