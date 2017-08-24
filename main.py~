# Assumptions:
"""
    10% of total energy is lost on every bounce
    Vertical bounces
    1 bounce takes 1 second
"""

# seconds
initial_time = 0.0
# meters
initial_height = 5.0
# kg
initial_mass = 0.02
# m/s
initial_velocity = 2.5
# m/s**2
gravitational_acceleration = 10.0


def calculate_displacement(v, t):
    return (v * t)


def calculate_time(s, v):
    return (s / v)


def calculate_velocity(s, t):
    return (s / t)


def calculate_potential_energy(m, g, h):
    return (m * g * h)


def calculate_height(pe, m, g):
    return (pe / (m * g))


def calculate_percent(value, percentage):
    return (value - (value * (float(percentage) / float(100))))


def bounce(no_of_bounces):
   
    m = initial_mass
    g = gravitational_acceleration
    h = initial_height
    v = initial_velocity
    t = initial_time
    pe = calculate_potential_energy(m, g, h) # PE at top

    for i in range(0, no_of_bounces, 1):
        t = t + 1
        pe = calculate_percent(pe, 10)
        v = calculate_velocity(h, t)
        h = calculate_height(pe, m, g)
        print("Height: {0}, Velocity: {1}, Time: {2}, PE: {3}".format(h, v, t, pe))
        print("--------")

bounce(3)






