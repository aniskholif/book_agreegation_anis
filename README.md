# book_agreegation_anis
class Book:
    def __init__(self, title, author, price):
        self.title = title
        self.author = author
        self.price = price

class Bookstore:
    def __init__(self, name):
        self.name = name
        self.books = []

    def add_book(self, book):
        self.books.append(book)

    def display_books(self):
        print("Daftar Buku di", self.name)
        print("--------------------")
        for book in self.books:
            print("Judul:", book.title)
            print("Penulis:", book.author)
            print("Harga:", book.price)
            print("--------------------")

# Membuat objek Bookstore
bookstore = Bookstore("Toko Buku safiQa")

# Membuat objek Book
book1 = Book("dilan", "pidi baiq", 9.99)
book2 = Book("rindu", "Tere liye", 5.99)
book3 = Book("tenggelamnya kapal van der wijck", "hamka", 7.99)

# Menambahkan objek Book ke dalam Bookstore
bookstore.add_book(book1)
bookstore.add_book(book2)
bookstore.add_book(book3)

# Menampilkan daftar buku yang tersedia di toko
bookstore.display_books()
