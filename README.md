# MatLab
# function text = double2eng(val, format)
% function TEXT = DOUBLE2ENG(VAL, FORMAT)
%   Creates a string with engineering units 'p', 'u' etc
%   VAL is the value to display and must be real non-vector
%   FORMAT is a string defining the format
%       Typical generic format would be '%4.2g%c'
%       For a capacitor, C = 34.5E-6 
%               txt = double2eng(34.5e-6, '%4.2g%cF')
%               txt gets '  34uF'
%       For a resistor of 6.85Meg you can use
%       txt = sprintf('%s%c', double2eng(6.85e6, '%4.3g'),937)
%               txt = '6.85M ohm' but the 937 character creates the ohm symbol
% Works for f (10^-15) to T (10^12)
% You can use this for the title of a figure plot as well
