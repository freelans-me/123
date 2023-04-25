class Database:
    def __init__(self, db_name):
        self.db_name = db_name
        self.connection = None
        
    def connect(self):
        # підключення до бази даних
        pass
    
    def disconnect(self):
        # відключення від бази даних
        pass
    
    def execute_query(self, query):
        # виконання запиту до бази даних
        pass
        
class WebScraper:
    def __init__(self, url):
        self.url = url
        self.html = None
        
    def fetch_html(self):
        # отримання HTML-коду
        pass
    
    def parse_html(self):
        # парсинг HTML-коду та отримання необхідної інформації
        pass
        
 class UserInterface:
    def __init__(self):
        self.menu = ["Option 1", "Option 2", "Option 3"]
        
    def display_menu(self):
        print("Menu:")
        for i, option in enumerate(self.menu):
            print(f"{i+1}. {option}")
            
    def get_user_choice(self):
        choice = input("Enter your choice: ")
        return choice
        
def run():
    db = Database("my_database")
    db.connect()
    db.execute_query("SELECT * FROM my_table")
    db.disconnect()
    
    scraper = WebScraper("https://www.example.com")
    scraper.fetch_html()
    scraper.parse_html()
    
    ui = UserInterface()
    ui.display_menu()
    choice = ui.get_user_choice()
    print(f"You chose option {choice}")
    
    if __name__ == "__main__":
    run()
