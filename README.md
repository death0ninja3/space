# space
"""
Realistic Solar System celestial catalog.
Distances (semi-major axis): AU (astronomical units)
Mass: kg
Radius: km
Mu (GM): m^3 / s^2 (Standard gravitational parameter)
Orbital Period: Earth years
"""

CELESTIAL_SYSTEM = {
    # -------------------------------------------------------------
    # 1. CENTRAL STAR
    # -------------------------------------------------------------
    "Sun": {
        "type": "star",
        "spectral_class": "G2V",
        "mass_kg": 1.9885e30,
        "radius_km": 696340.0,
        "mu_m3_s2": 1.32712440018e20,
        "rotation_period_days": 25.05,
        "color_hex": "#FFF4E8",
        "a_au": 0.0,
        "eccentricity": 0.0,
        "inclination_deg": 0.0,
        "orbital_period_yr": 0.0,
    },

    # -------------------------------------------------------------
    # 2. TERRESTRIAL PLANETS
    # -------------------------------------------------------------
    "Mercury": {
        "type": "major_planet",
        "mass_kg": 3.3011e23,
        "radius_km": 2439.7,
        "mu_m3_s2": 2.2032e13,
        "a_au": 0.387098,
        "eccentricity": 0.205630,
        "inclination_deg": 7.005,
        "orbital_period_yr": 0.2408,
        "color_hex": "#8C8C8C",
    },
    "Venus": {
        "type": "major_planet",
        "mass_kg": 4.8675e24,
        "radius_km": 6051.8,
        "mu_m3_s2": 3.24859e14,
        "a_au": 0.723332,
        "eccentricity": 0.006773,
        "inclination_deg": 3.39458,
        "orbital_period_yr": 0.6152,
        "color_hex": "#E3BB7B",
    },
    "Earth": {
        "type": "major_planet",
        "mass_kg": 5.9722e24,
        "radius_km": 6371.0,
        "mu_m3_s2": 3.986004418e14,
        "a_au": 1.000000,
        "eccentricity": 0.0167086,
        "inclination_deg": 0.00005,
        "orbital_period_yr": 1.0000,
        "color_hex": "#4B70DD",
    },
    "Mars": {
        "type": "major_planet",
        "mass_kg": 6.4171e23,
        "radius_km": 3389.5,
        "mu_m3_s2": 4.282837e13,
        "a_au": 1.523679,
        "eccentricity": 0.0934,
        "inclination_deg": 1.850,
        "orbital_period_yr": 1.8808,
        "color_hex": "#C1440E",
    },

    # -------------------------------------------------------------
    # 3. ASTEROID BELT (DWARF PLANET)
    # -------------------------------------------------------------
    "Ceres": {
        "type": "dwarf_planet",
        "mass_kg": 9.3835e20,
        "radius_km": 469.7,
        "mu_m3_s2": 6.263e10,
        "a_au": 2.7675,
        "eccentricity": 0.0758,
        "inclination_deg": 10.593,
        "orbital_period_yr": 4.60,
        "color_hex": "#9E9993",
    },

    # -------------------------------------------------------------
    # 4. GAS GIANTS
    # -------------------------------------------------------------
    "Jupiter": {
        "type": "major_planet",
        "mass_kg": 1.8982e27,
        "radius_km": 69911.0,
        "mu_m3_s2": 1.26686534e17,
        "a_au": 5.204267,
        "eccentricity": 0.048498,
        "inclination_deg": 1.303,
        "orbital_period_yr": 11.862,
        "has_rings": True,
        "color_hex": "#D8CA9D",
    },
    "Saturn": {
        "type": "major_planet",
        "mass_kg": 5.6834e26,
        "radius_km": 58232.0,
        "mu_m3_s2": 3.7931187e16,
        "a_au": 9.53707,
        "eccentricity": 0.05555,
        "inclination_deg": 2.485,
        "orbital_period_yr": 29.457,
        "has_rings": True,
        "color_hex": "#E2BF7D",
    },

    # -------------------------------------------------------------
    # 5. ICE GIANTS
    # -------------------------------------------------------------
    "Uranus": {
        "type": "major_planet",
        "mass_kg": 8.6810e25,
        "radius_km": 25362.0,
        "mu_m3_s2": 5.793939e15,
        "a_au": 19.19126,
        "eccentricity": 0.047318,
        "inclination_deg": 0.772,
        "orbital_period_yr": 84.011,
        "axial_tilt_deg": 97.77,
        "has_rings": True,
        "color_hex": "#BBE1E4",
    },
    "Neptune": {
        "type": "major_planet",
        "mass_kg": 1.02413e26,
        "radius_km": 24622.0,
        "mu_m3_s2": 6.836529e15,
        "a_au": 30.06896,
        "eccentricity": 0.008678,
        "inclination_deg": 1.769,
        "orbital_period_yr": 164.79,
        "has_rings": True,
        "color_hex": "#6081FF",
    },

    # -------------------------------------------------------------
    # 6. RECOGNIZED TRANS-NEPTUNIAN DWARF PLANETS
    # -------------------------------------------------------------
    "Pluto": {
        "type": "dwarf_planet",
        "mass_kg": 1.303e22,
        "radius_km": 1188.3,
        "mu_m3_s2": 8.71e11,
        "a_au": 39.482,
        "eccentricity": 0.2488,
        "inclination_deg": 17.16,
        "orbital_period_yr": 247.94,
        "color_hex": "#D1B59B",
    },
    "Haumea": {
        "type": "dwarf_planet",
        "mass_kg": 4.006e21,
        "radius_km": 798.0,  # Mean volumetric radius (triaxial: 1050 x 840 x 537 km)
        "mu_m3_s2": 2.674e11,
        "a_au": 43.218,
        "eccentricity": 0.1912,
        "inclination_deg": 28.19,
        "orbital_period_yr": 283.84,
        "has_rings": True,
        "color_hex": "#A7A59B",
    },
    "Makemake": {
        "type": "dwarf_planet",
        "mass_kg": 3.1e21,
        "radius_km": 715.0,
        "mu_m3_s2": 2.07e11,
        "a_au": 45.79,
        "eccentricity": 0.1559,
        "inclination_deg": 28.96,
        "orbital_period_yr": 306.17,
        "color_hex": "#C78B63",
    },
    "Quaoar": {
        "type": "dwarf_planet",
        "mass_kg": 1.2e21,
        "radius_km": 555.0,
        "mu_m3_s2": 8.0e10,
        "a_au": 43.69,
        "eccentricity": 0.038,
        "inclination_deg": 7.99,
        "orbital_period_yr": 288.0,
        "has_rings": True,
        "color_hex": "#8C6A58",
    },
    "Eris": {
        "type": "dwarf_planet",
        "mass_kg": 1.66e22,
        "radius_km": 1163.0,
        "mu_m3_s2": 1.108e12,
        "a_au": 67.781,
        "eccentricity": 0.4407,
        "inclination_deg": 44.04,
        "orbital_period_yr": 558.04,
        "color_hex": "#EFEFEF",
    },

    # -------------------------------------------------------------
    # 7. HIGH-PROBABILITY DWARF PLANET CANDIDATES
    # -------------------------------------------------------------
    "Orcus": {
        "type": "candidate_dwarf_planet",
        "mass_kg": 6.32e20,
        "radius_km": 458.0,
        "mu_m3_s2": 4.2e10,
        "a_au": 39.419,
        "eccentricity": 0.2255,
        "inclination_deg": 20.58,
        "orbital_period_yr": 247.5,
        "color_hex": "#707372",
    },
    "Salacia": {
        "type": "candidate_dwarf_planet",
        "mass_kg": 4.92e20,
        "radius_km": 423.0,
        "mu_m3_s2": 3.28e10,
        "a_au": 42.18,
        "eccentricity": 0.106,
        "inclination_deg": 23.94,
        "orbital_period_yr": 274.0,
        "color_hex": "#504E4D",
    },
    "2002_MS4": {
        "type": "candidate_dwarf_planet",
        "mass_kg": 4.0e20,
        "radius_km": 400.0,
        "mu_m3_s2": 2.67e10,
        "a_au": 41.93,
        "eccentricity": 0.148,
        "inclination_deg": 17.70,
        "orbital_period_yr": 271.5,
        "color_hex": "#6B6560",
    },
    "Gonggong": {
        "type": "candidate_dwarf_planet",
        "mass_kg": 1.75e21,
        "radius_km": 615.0,
        "mu_m3_s2": 1.17e11,
        "a_au": 67.48,
        "eccentricity": 0.500,
        "inclination_deg": 30.74,
        "orbital_period_yr": 554.2,
        "color_hex": "#A84C38",
    },
    "Sedna": {
        "type": "candidate_dwarf_planet",
        "mass_kg": 2.0e21,
        "radius_km": 500.0,
        "mu_m3_s2": 1.33e11,
        "a_au": 525.86,
        "eccentricity": 0.855,
        "inclination_deg": 11.93,
        "orbital_period_yr": 11400.0,
        "color_hex": "#B0422B",
    },
}
