# Hotel Management System (C++)

A console-based hotel management system written in C++. Guest data, room inventory, reservations, and restaurant orders are all persisted to plain-text files so state survives between runs.

## Features

- **Room management** — add, search, delete, and display rooms by type and availability
- **Guest check-in / check-out** — records guest details, room assignment, and billing
- **Reservations** — create and track bookings with date-based lookup
- **Restaurant menu** — order food from an in-app menu; cost added to guest bill
- **Admin panel** — protected admin access for hotel and staff management
- **Ratings and feedback** — guests can leave reviews stored to file
- **File persistence** — all data written to `.txt` files (`rooms.txt`, `reservations.txt`, `users.txt`, ...)

## Project structure

```
├── hotelreservationsystemm.cpp   # Full application source
├── rooms.txt                     # Room inventory (runtime data)
├── reservations.txt              # Booking records
├── users.txt                     # Registered users
├── admins.txt                    # Admin credentials
├── menu.txt                      # Restaurant menu items
├── services.txt                  # Additional services
├── hotel_ratings.txt             # Guest ratings
└── feedback.txt                  # Guest feedback
```

## Build and run

```bash
g++ -o hotel hotelreservationsystemm.cpp
./hotel
```

Requires a C++11-compatible compiler. On Windows, compile with MinGW or MSVC.

## Tech stack

- **C++** — core language
- **File I/O** — plain-text persistence (`fstream`)
- **OOP** — structs for Room, Hotel, Guest, Food entities
