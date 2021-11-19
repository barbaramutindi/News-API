import unittest
from .models import source

Source = source.Source

class SourceTest(unittest.TestCase):
    '''
    Test class to test the behaviour of the news class
    '''
    def setUp(self):
        '''
        Method to run before every Test
        '''
        self.new_source= Source( "cbs-news","CBS News","A grocery store employee was killed in a shooting at a Stop & Shop on New York's Long Island Tuesday morning, police said.","https://www.cbsnews.com/live-updates/stop-and-shop-shooting-west-hempstead-new-york/","general")
        
    def test_instance(self):
        self.assertTrue(isinstance(self.new_source,Source))

if __name__ == '__main__':
    unittest.main()
    