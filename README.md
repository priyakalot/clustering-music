# Clustering Music into Genres
# Research for Industrial Projects for Students (RIPS) Hong Kong 2018
# Industry Sponsor: Tencent

This project is part of the RIPS-HK program, and was sponsored by Tencent. The project was a collaborative effort by Gabrielle Ferra (Brown University), Algor Lin (Hong Kong University of Science and Technology), Harrison Huang (Hong Kong University of Science and Technology), and me (UCLA).

We were mentored by Professor Yu-Wing Tai and Bhaven Mistry.

This code represents one part of the overall project. This part focuses on clustering music (in MIDI files) into groups representing genres. We extracted information from the state matrix representation of musical pieces (found here: https://github.com/hexahedria/biaxial-rnn-music-composition/blob/master/midi_to_statematrix.py) to create vector representations of pieces to cluster using the k-means algorithm. (Please note that our code relies on a few functions from the earlier mentioned Github. The functions from "midi_to_statematrix.py" will suffice.)

The features we used to define a piece of music are as follows:

1. Total number of plays
2. Total number of articulations
3. Total number of articulations and plays
4. Average number of plays per time step
5. Average number of articulations per time step
6. Average number of articulations and plays per time step
7. Number of notes (out of 78) not played
8. Length of the piece of music
