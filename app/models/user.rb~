class User < ActiveRecord::Base
  attr_accessible :email, :name
  has_many :microposts
  validates_numericality_of :citizen_id, :only_integer => true, :allow_nil => false, :if => Proc.new{|user| !user.citizen_id.blank?}

end
