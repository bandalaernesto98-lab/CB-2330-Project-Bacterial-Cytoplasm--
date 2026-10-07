alpha = 0.7

Random generator:
rng = np.random.default_rng() # generates a random number

We adapted the paper's power law to randomly predict the amount of time our observed particle becomres trapped.
P(t_c) ~ t_c^(−ν), and then α = ν − 1

Code representation of the cage time adapted eqation:
next_jump = 0.1 * (1 - rng.random()) ** (-1/(v-1))   # 0.1 s is the shortest possible trap

The distribution of the particules movement was assumed to be a Gaussian distribution for coding simplicity and then randomnized
for i in range(video_length):                         # the camera clock Starts at with a trap - an assuption/limitation.
        while next_jump <= i:                             # has the trap ended yet?
            x = x + rng.normal(0, sigma)                  # jump, typical size sigma
            y = y + rng.normal(0, sigma)
            next_jump = next_jump + 0.1 * (1 - rng.random()) ** (-1/(v-1))   # schedule the next jump

