```Ruby
class SoftwareEngineer < Person
  attr_reader :years_professional

  def initialize(name:, place_of_birth:, birthdate:)
    super(name: name, place_of_birth: place_of_birth, birthdate: birthdate)
  end

  def greeting
    super # 👋 Hi, I’m @petertimwalker from Boston MA and I'm 26 years old
    puts "I've been working professionally for the past #{years_professional} years"
    puts "and I'm interested in Ruby, React, AWS, and Docker"
  end

  private

  def years_professional
    @years_professional ||= 4
  end
end

```
