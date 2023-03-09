# Stranger-Things
notes = [:c2, :e2, :g2, :b2, :c3, :b2, :g2, :e2]
i = 0

use_bpm 160
use_synth :saw

live_loop :main_theme do
  with_fx :distortion do
    8.times do
      puts(i)
      play(notes[i])
      sleep 0.5
      i = i + 1
    end
    i = 0
  end
end
