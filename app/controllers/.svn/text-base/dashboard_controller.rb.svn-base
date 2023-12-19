
class DashboardController < ActionController::Base
  
  
  def welcome
    
  end

  def show_most_sold_products
    @most_sold_yesterday = Product.find_by_sql("select link,sold,maxsoldday,leastsoldday,updated,localcost from products where (leastsoldday>0) and (leastsoldday<2147483647) order by maxsoldday desc limit 100;")
    puts @most_sold_yesterday.to_s
    
  end

  def show_most_sold_yesterday
    #where (DATE_SUB(DATE(NOW()),INTERVAL 1 DAY) = DATE(updated)) 
    @most_sold_yesterday = Product.find_by_sql("select * from products limit 10;")
    
  end

  def calculate_suggestions
    
    
  end
  
  def show_investment_form
    
    
  end
  
  def show_questions
    
  end
  
  def order_log
    
  end
  
end